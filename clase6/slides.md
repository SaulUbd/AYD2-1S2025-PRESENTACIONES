---
theme: mint
title: DevOps
image: ./assets/cover-meme-stretched.jpg
---

# DevOps
Análisis y Diseño de Sistemas 2
Saul Castellanos

---
layout: image
image: ./assets/deploy-on-friday.jpg
backgroundSize: contain
---
---

# DevOps? kesesotu?
## ¿Con qué se come?
### No, de verdad ¿Qué es?
#### ¿Y quién soy yo?

DevOps (Development Operations) es un conjunto de prácticas y herramientas que busca incrementar la eficiencia y velocidad de el desarrollo de software y su entrega/despliegue.
Se trata de la integración y automatización de el desarrollo de software y operaciones de tecnología de la información.

Una definición sugerida es:
> Un conjunto de prácticas que pretenden reducir el tiempo entre realizar un cambio dentro de un sistema y ese cambio siento integrando en el entorno de producción normal, al mismo que tiempo que se asegura alta calidad.

<!--
DevOps is the integration and automation of the software development and information technology operations[a]. DevOps encompasses necessary tasks of software development and can lead to shortening development time and improving the development life cycle.[1] According to Neal Ford, DevOps, particularly through continuous delivery, employs the "Bring the pain forward" principle, tackling tough tasks early, fostering automation and swift issue detection.[2] Software programmers and architects should use fitness function to keep their software in check.[3]

Although debated,[b][c][d][e] DevOps is characterized by key principles: shared ownership, workflow automation, and rapid feedback. From an academic perspective, Len Bass, Ingo Weber, and Liming Zhu—three computer science researchers from the CSIRO and the Software Engineering Institute—suggested defining DevOps as "a set of practices intended to reduce the time between committing a change to a system and the change being placed into normal production, while ensuring high quality".[7] However, the term is used in multiple contexts. At its most successful, DevOps is a combination of specific practices, culture change, and tools.[8] 
-->

---

# DevOps
## Ciclo de vida
[fuente*](https://medium.com/edureka/devops-lifecycle-8412a213a654)

En general, DevOps puede ser descrito como una serie de fases. A esto se le llama el ciclo de vida DevOps.

- Continuous development (Desarrollo continuo)
- Continuous testing (Pruebas continuas)
- Continuous integration (Integración continua)
- Continuous deployment (Despliege continuo)
- Continuous monitoring (Monitoreo continuo)

_CI/CD_ hace referencia a las fases de "continuous integration" y "continuous deployment" de forma automatizada.

---
layout: image
image: ./assets/devops-cycle.webp
backgroundSize: contain
---
---
layout: two-cols-header
---

# DevOps
## Ciclo de vida DevOps
### Desarrollo continuo

::left::

### Planeación
- En este paso se define la visión para el proyecto y para cada iteración.
- No hay herramientas especificas para esto.
- Aquí también definiriamos la metodología para el desarrollo (Ágil, cascada, etc.)

::right::

### Desarrollo
- En este paso se desarrolla la aplicación.
- Se utiliza herramientas de control de versiones para el control y mantenimiento del código.

<!--
This is the phase that involves ‘planning’ and ‘coding’ of the software. The vision of the project is decided during the planning phase and the developers begin developing the code for the application. There are no DevOps tools that are required for planning, but there are a number of tools for maintaining the code.

The code can be written in any language, but it is maintained by using Version Control tools. Maintaining the code is referred to as Source Code Management. The most popular tools used are Git, SVN, Mercurial, CVS, and JIRA. Also tools like Ant, Maven, Gradle can be used in this phase for building/ packaging the code into an executable file that can be forwarded to any of the next phases.

- Plan – The planning phase is exactly what it sounds like: planning the project’s lifecycle. In contrast to conventional methods to the development lifecycle, this model assumes that each stage will be repeated as necessary. In this manner, the DevOps workflow is planned with the likelihood of future iterations and likely prior versions in mind.This implies that we will likely have information from past iterations that will better inform the next iteration, and that the present iteration will likewise inform the next iteration. This stage often involves all teams to ensure that no area of the planning is ignored or forgotten.

- Code – The developers will write the code and prepare it for the next phase during the coding stage. Developers will write code in accordance with the specifications outlined in the planning phase and will ensure that the code is created with the project’s operations in mind.
-->

---
layout: two-cols-header
---

# DevOps
## Ciclo de vida DevOps
### Pruebas continuas

::left::

### Build
- Introducción del código al proyecto
- Requiere revisión y aprobación

::right::

### Test

- Todas las pruebas necesarias para asegurar el funcionamiento del proyecto
- Aquí es donde se trabaja lo de QA

<!--
This is the stage where the developed software is continuously tested for bugs. For Continuous testing, automation testing tools like Selenium, TestNG, JUnit, etc are used. These tools allow QAs to test multiple code-bases thoroughly in parallel to ensure that there are no flaws in the functionality. In this phase, Docker Containers can be used for simulating the test environment.

- Build – Code will be introduced to the project during the construction phase, and if necessary, the project will be rebuilt to accommodate the new code. This can be accomplished in a variety of ways, although GitHub or a comparable version control site is frequently used.The developer will request the addition of the code, which will then be reviewed as necessary. The request will be approved if the code is ready to be uploaded, and the code will be added to the project. Even when adding new features and addressing bugs, this method is effective.

- Test – Throughout the testing phase, teams will do any necessary testing to ensure the project performs as planned. Teams will also test for edge and corner case issues at this stage. An “edge case” is a bug or issue that only manifests during an extreme operating event, whereas a “corner case” occurs when many circumstances are met.
-->

---
layout: image-right
image: ./assets/ci.jpg
---

# DevOps
## Ciclo de vida DevOps
### Integración continua

Esta fase es el corazón del ciclo de vida DevOps. A partir del resultado de las fases anteriores, se crean nuevos releases que serán destinados a ser desplegados en el entorno de producción.

<!--
This stage is the heart of the entire DevOps life cycle. It is a software development practice in which the developers require to commit changes to the source code more frequently. This may be on a daily or a weekly basis. Every commit is then built and this allows early detection of problems if they are present. Building code not only involves compilation but it also includes code review, unit testing, integration testing, and packaging.

The code supporting new functionality is continuously integrated with the existing code. Since there is continuous development of software, the updated code needs to be integrated continuously as well as smoothly with the systems to reflect changes to the end-users.

- The release phase occurs when the code has been verified as ready for deployment and a last check for production readiness has been performed. The project will subsequently enter the deployment phase if it satisfies all requirements and has been thoroughly inspected for bugs and other problems.
-->

---
layout: two-cols-header
---

# DevOps
## Ciclo de vida DevOps
### Despliegue continuo

::left::

### Despliegue

- Despliegue de la aplicación en el entorno de producción
- Manejo de configuración para entornos
- Contenerización

::right::

### Operación

- Probar la aplicación en el entorno de producción
- Usuarios interactuan con la aplicación

<!--
This is the stage where the code is deployed to the production servers. It is also important to ensure that the code is correctly deployed on all the servers. Before moving on, let us try to understand a few things about Configuration management and Containerization tools. These set of tools here help in achieving Continuous Deployment (CD).

Configuration Management is the act of establishing and maintaining consistency in an application’s functional requirements and performance. Let me put this in simpler words, it is the act of releasing deployments to servers, scheduling updates on all servers and most importantly keeping the configurations consistent across all the servers.

Since the new code is deployed on a continuous basis, configuration management tools play an important role in executing tasks quickly and frequently. Some popular tools that are used here are Puppet, Chef, SaltStack, and Ansible.

Containerization tools also play an equally important role in the deployment stage. Docker and Vagrant are the popular tools used for this purpose. These tools help produce consistency across Development, Test, Staging and Production environments. Besides this, they also help in scaling-up and scaling-down of instances swiftly.

Containerization tools help in maintaining consistency across the environments where the application is developed, tested and deployed. Using these tools, there is no scope of errors/ failure in the production environment as they package and replicate the same dependencies and packages used in the development/ testing/ staging environment. It makes your application easy to run on different computers.

- Deploy – In the deploy phase, the project is prepared for the production environment and is operating as planned in that environment. This would be the responsibility of the operations team; in DevOps, it is a shared responsibility. This shared duty pushes team members to collaborate to guarantee a successful deployment.

- Operate – In the operating phase, teams test the project in a production environment, and end users utilise the product. This crucial stage is by no means the final step. Rather, it informs future development cycles and manages the configuration of the production environment and the implementation of any runtime requirements.
-->

---
layout: image-left
image: ./assets/monitoring.jpg
---

# DevOps
## Ciclo de vida DevOps
### Monitoreo continuo

En esta fase se monitorea el desempeño de la aplicación. Es la fase donde se reconoce y documenta cualquier retroalimentación, problema u oportunidad de mejora.

<!--
This is a very crucial stage of the DevOps life cycle where you continuously monitor the performance of your application. Here vital information about the use of the software is recorded. This information is processed to recognize the proper functionality of the application. The system errors such as low memory, server not reachable, etc are resolved in this phase.

The root cause of any issue is determined in this phase. It maintains the security and availability of the services. Also if there are network issues, they are resolved in this phase. It helps us automatically fix the problem as soon as they are detected.

This practice involves the participation of the Operations team who will monitor the user activity for bugs or any improper behavior of the system. The popular tools used for this are Splunk, ELK Stack, Nagios, NewRelic and Sensu. These tools help you monitor the application’s performance and the servers closely and also enable you to check the health of the system proactively.

They can also improve productivity and increase the reliability of the systems, which in turn reduces IT support costs. Any major issues if found are reported to the development team so that it can be fixed in the continuous development phase. This leads to a faster resolution of the problems.

- Monitor – During the monitoring phase, product usage, as well as any feedback, issues, or possibilities for improvement, are recognized and documented. This information is then conveyed to the subsequent iteration to aid in the development process. This phase is essential for planning the next iteration and streamlines the pipeline’s development process.
-->

---

# DevSecOps
## Ni modo que dejemos todo expuesto, bro
[fuente*](https://www.atlassian.com/devops/devops-tools/devsecops-tools)

DevSecOps (Development Security Operations) hace referencia a la aplicación de medidas de seguridad en cada una de las fases del ciclo de vida DevOps. No es diferente a DevOps, sino que se trata de asegurar cada fase de DevOps. Cuando una empresa/proyecto implementa DevOps o habla de DevOps, muy probablemente está hablando de DevSecOps.

---
layout: image
image: ./assets/DevSecOps-cycle.png
backgroundSize: contain
---

<!--
Dynamic Application Security Testing (DAST) es el proceso de usar ataques simulados en una aplicación web para identificar vulnerabilidades. Al atacar una aplicación de la misma manera que lo haría un usuario malicioso, esta estrategia evalúa el programa a través de un enfoque que a veces se denomina “de afuera hacia adentro”. Después de ejecutar los ataques, un escáner DAST estudia los resultados para buscar resultados no deseados. Estos datos luego se utilizan para identificar fallas de seguridad.

# DAST

La capacidad de DAST para utilizar el análisis dinámico de código para detectar problemas de tiempo de ejecución, debilidades que no se pueden ver cuando un programa no se está ejecutando, es una de sus principales ventajas. El DAST también examina cómo una aplicación  responde realmente a un ataque, proporcionando información valiosa sobre la probabilidad de que se aproveche una vulnerabilidad.

# SAST

SAST es excelente para encontrar vulnerabilidades a medida que se produce el código. Sin SAST, es probable que un equipo de desarrollo no detecte problemas hasta más adelante en el ciclo de vida del desarrollo de software (SDLC). Además, SAST puede identificar errores de codificación, lo que facilita que los desarrolladores identifiquen y aborden las vulnerabilidades.
-->

---

# DevOps
## Beneficios

- Automatización
- Equipos de desarrollo y de operaciones no están aislados. La responsabilidad de la entrega de software es compartida.
- Menor fricción entre los equipos
- Mayor velocidad en la entrega de software
- Mayor facilidad para la innovación

<!--
Adopting DevOps breaks down barriers so that development and operations teams are no longer siloed and have a more efficient way to work across the entire development and application lifecycle. Without DevOps, organizations often experience handoff friction, which delays the delivery of software releases and negatively impacts business results.

The DevOps model is an organization’s answer to increasing operational efficiency, accelerating delivery, and innovating products. Organizations that have implemented a DevOps culture experience the benefits of increased collaboration, fluid responsiveness, and shorter cycle times.
-->

---
layout: center
---

# Herramientas

---
layout: image
image: ./assets/tools.webp
backgroundSize: contain
---
