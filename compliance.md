# Software y cumplimiento

Seguramente el cumplimiento de la normativa se siente como algo incómodo, un mal necesario, algo que si pudiéramos evitar, lo evitaríamos. Entiendo que la regulación está pensada, en buena parte, para proteger. Como por ejemplo la RGPD y la LOPDGDD están para que no puedas hacer lo que te de la gana con los datos personales.

Sin embargo en software tenemos tendencia a motivarnos solo con las cosas nuevas y sofisticadas y lo aburrido que lo haga otro. También es verdad que hay mucha gente que disfruta con cosas como mantener en buena forma sistemas heredados, algo que en principio puede resultar poco atractivo. Y por otro lado tenemos el contrapeso de quien afirma, sin pestañear, que le cuesta menos la multa, si es que algún día llega, que implementar al pie de la letra la regulación.

Cuando estudias marketing, administración de empresas, etc, a parte del DAFO siempre te piden el PESTEL, que sirve para entender mínimamente el entorno del sector en el que está la empresa; la L hace referencia a los factores legales. La parte de ingeniería de nuestro oficio es esto, es entender también que el software tiene que ser viable con lo cual necesitas entender el marco legal que a su vez te lleva a entender mejor el negocio en general.

Integrar el cumplimiento de la normativa en el SDLC no es solo un requisito sino una oportunidad de que los equipos que hacen software sean mejores, dotando a la tecnología que desarrollan de una base impecable, sin limitarnos a nosotros mismos pensando que eso es cosa de bancos. Con lo cual yo invito a todas las personas que se dedican a esto que lo incorporen sin esperar a que "el de compliance" le pida unos cambios al product manager y etc.

## Riesgos

Si lo primero que pensamos cuando ponemos el cumplimiento sobre la mesa es de cuánto es la multa y qué posibilidades hay de que me pillen creo que no lo estamos enfocando bien. La otra vertiente está en el riesgo de perjudicar los derechos de tus clientes. De una forma u otra, no cumplir tiene riesgos, que hay que gestionar independientemente de su naturaleza. Pero desde el punto de vista tecnológico y de producto, me parece mucho más interesante gestionar los riesgos pensando en tus clientes y usuarios que pensando en protegerte (de las consecuencias de no hacer lo que tienes que hacer).

En salud el impacto del incumplimiento es tal que te puede sacar del mercado directamente y en ese caso tienes un problema mucho más que económico. Nos pasa que en otras verticales el impacto puede parecer bajo; todo depende de cómo vayas de caja. En una startup que normalmente no tiene a nadie dedicado a estos temas porque se lo suele llevar una agencia (que básicamente prepara los textos legales) y le está costando la vida encontrar su lugar en el mundo, una sanción por incumplimiento igual no la deja fuera del juego pero sí le puede reducir uno o dos meses el runway. Así que no es ninguna tontería.

Pienso que muchas organizaciones que hacen software deberían aprender a gestionarse en base a riesgos para adquirir consciencia del mundo en el que viven y de las implicaciones de hacer o dejar de hacer según qué cosas.

## SDLC

La suerte que tenemos de vivir la época que estamos viviendo es que el coste de mitigar los riesgos asociados al incumplimiento están bajando a medida que los LLM se hacen más expertos y, lo mejor de todo, es que puedes automatizarlo e incorporarlo en tu SDLC con poco esfuerzo y mucha solvencia &mdash; continuous compliance.

Por ejemplo, este es un informe generado con Claude Sonnet después de contrastar el código fuente de un proyecto en fase muy inicial con los principios y requerimientos de la RGPD:

```
Most Critical Issues:

1. Unencrypted In-Memory Storage - User data stored in plain Python dictionaries without encryption
2. GitHub Tokens Stored Without Encryption - OAuth tokens vulnerable in sessions
3. PII Sent to Sentry - User data exposed to third-party error tracking service
4. User Profile Bug - Undefined variable causes crashes and data loss
5. HTTPS Disabled - Sessions transmitted without encryption in production

Key Compliance Gaps:

- No Data Subject Rights Implementation - Users can't exercise their GDPR rights (access, deletion, portability, etc.)
- No Consent Management - No cookie consent or explicit consent collection
- No Data Retention Policies - Data kept indefinitely
- Missing Documentation - No Privacy Policy, DPIA, or Data Processing Agreements
- No Audit Logging - Cannot track who accessed what data when

Required Actions Before Production:

Immediate:
- Fix the user profile bug (undefined variable)
- Enable HTTPS on load balancer and sessions
- Disable Sentry PII sending
- Remove mock users from code

Before Accepting Users:
- Implement data subject access/deletion endpoints
- Create Privacy Policy and Cookie Consent
- Establish Data Processing Agreements
- Migrate from in-memory to encrypted database storage
- Implement comprehensive audit logging
```

Comparad esto con lanzar una consulta por email al profesional de referencia que responderá cuando buenamente pueda con lo que buenamente entiende o conoce de tu producto. Yo no lo desaprovecharía. Y las asesorías o despachos que se dediquen a estas cosas pueden aprovecharlo también, pero eso es harina de otro costal que queda bastante lejos de mis competencias.

## Conclusión

Me he puesto muy intenso con la normativa de obligado cumplimiento pero hay otros marcos que son voluntarios y de los que pienso lo mismo: nos ayudan a hacer mejor software siempre y cuando nos lo tomemos como algo potenciador, no como un obstáculo. En general mi postura es siempre la misma: la tecnología que vendes directamente o el servicio que prestas a través de tu tecnología no puede tener puntos débiles porque bastante difícil es vender como para que el software no esté preparado para ser comercializado. Y si cojea, lo mejor que se puede hacer es tener un plan.
