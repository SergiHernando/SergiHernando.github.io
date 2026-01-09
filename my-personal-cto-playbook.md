# My Personal CTO Playbook (That I Wish I Had When I Started)

> [!NOTE]
> Rough draft

> [!IMPORTANT]
> Human-generated content

A veces me he preguntado: cuál es mi método. Siempre respondía: depende del contexto. Lo cierto es que no es así. Es decir, el camino que voy a tomar sí que depende del contexto, pero la aproximación a los problemas o condicionantes tiene ciertos patrones que he repetido en cada situación.

Based on my experience leading technology at startup ventures in their 0 to 1 and 1 to 10 growth stages, pre-series A and post-PMF, this is the playbook I wish I had when I started in 2010 my own leadership path.

## Responsibilities

Time frame is between next year and the other next:

- **Budget**: How much money can we spend. Easy question, difficult answer. Specially difficult for leadership who's not used to make bets. They'll have a tendency to demand dates along with a list of features. I respond: What do we need to achieve in terms of business outcomes? With that I try to force a discussion with the founders so that everybody understands what should be the investment and why.

  Heads up: I won't consider myself a CTO if I can't manage a budget. Chiefs without budget are not chiefs. Strong opinion here.

- **Teams**: Once we know the money, I can draft a plan. My plans do not include tasks, assignments nor milestones. It's a matter of hiring the right people to execute today and to be ready for next stage tomorrow. What do I look in candidates? (1) People whom I share that working software is the only measure of progress, (2) People that take nothing for granted, and (3) People that are willing to niteract with other people in the organization regardless of their roles.

- **Technology**: This is the obvious part, but I have to beat some intermediate monsters yet. Being the technology leader is my responsibility to research and build exactly what's important for the bussiness to move forward. Tough but mandatory to push back engineers' ideas to implement this or that that does not clearly solves a business case.

## Heuretics

### Reglas no escritas

Todos los negocios tienen una idiosincrasia, una razón de ser o unas líneas rojas que, especialmente en fases iniciales, no siempre se expresan explícitamente verbalmente o por escrito. Una de las primeras cosas que hago es identificar esos códigos y trasladarlos a unos principios que deben guiar a mis equipos ante la duda.

Un par de ejemplos serían los siguientes. Si la empresa está en FinTech y el producto básicamente hace operaciones aritméticas con decimales, trasladaría eso a un valor del equipo: la precisión. Si el producto está en un entorno regulado como en HealthTech, un valor del equipo sería la trazabilidad – todo lo que hacemos debe quedar registrado, cuándo, por quién y por qué.

Tengo siempre en cuenta también que esto puede cambiar con el tiempo. Me gusta cuestionar los valores que las empresas publican: talento, calidad, innovación… Alguien piensa que sin personas se puede construir algo? Y algo que no satisface correctamente su utilidad? Y alguna empresa prefiere estancarse tecnológicamente? Por supuesto que no. Con lo cual, creo que los valores son de todo menos obvios. Y es imposible describirlos de antemano.

### Software

Tomar decisiones de arquitectura que no limiten/impidan/condicionen el futuro de la empresa.

Although business goes into software and we use software for building everything, software is just a part. For building software properly, to me it's fundamental that the following also happens:

- There's a **shared understanding** of the problems we are trying to solve among all the stakeholders.

- There's a **technical infrastructure** that has to be built.

- There are well-known **communication channels** and a **communication etiquette** in place. I try to be rigorous in how I communicate with those around me. While I greatly value informal, unstructured conversations, I need the information shared in those conversations to be preserved. Therefore, for me, both the channel and the method are important.

Depending on the objective ahead, I may need to write a lot of code just like anyone else. Even though that swallows large amounts of attention, I need to find a way to be aware of what's going on and know all the details. What do I use for that purpose?

- **Asynchronous code reviews with the scout hat on**, absolutely no intention to blame nobody. Actually, if a find a piece of code that for example does not adhere to this or that code conventions is actually my fault, not the author's.

- **Regular conversations with direct reports and peer managers**. I don't use a template to conduct 1:1 meetings and I let conversations naturaly navigate recent events. Structured 1:1's give me the impression of being somewhat forced, whereas I want them to be the complete opposite.

- **Sharing in-depth periodic updates with the entire organization**. This includes the publication of postmortems: If part or all of the system goes down, affecting customers, coworkers, or both, I always explain what happened, why it happened, and what we're going to do to prevent it from happening again.

### Working with me

I don't expect people to do any overtime. De hecho espero que la empresa sea lo suficientemente madura como para entender que encorsetar el trabajo creativo en una estructura horaria rígida.

### A brief note about remote work

I don't have a strong opinion here.

### Metrics

I'm skeptical of most engineering metrics I see companies tracking. Thinking of DORA and the like. All of that tells you nothing about whether you're moving the business forward. I want metrics to be a measure (even temporary) to improve the system itself, and for god's sake **never tied to team or individual performance**. What I do believe in: SLAs and SLOs. That is: the intersection of the commitments with ourselves and with our customers.

So, Sergi, how do you do performance appraisal? I don't. Career paths, to my understanding, must be defined around the problems and challenges people face and whether they are successful in dealing with them or not.

## Commandments

- Infrastructure is an intrinsic part of the product.
- I don't have all the answers but most importantly: I don't want to.
