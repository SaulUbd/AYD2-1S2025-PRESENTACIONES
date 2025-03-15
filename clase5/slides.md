---
theme: mint
title: Pruebas de software
image: ./assets/cover-meme.jpg
---

# Pruebas de software
Análisis y Diseño de Sistemas 2
Saul Castellanos

---
layout: two-cols-header
---

# Pruebas de software
[fuente*](https://en.wikipedia.org/wiki/Software_testing)

Realizar pruebas de software es el acto de verificar que el software satisface las espectativas.
Normalmente responde a las preguntas:

- ¿Hace el software lo que se supone que debe hacer? (¿Funciona como debe?)
- ¿Hace el software lo que tiene que hacer? (¿Cumple con el diseño/intención?)

::left::

## Pruebas funcionales

Son pruebas que verifican acciones especificas o funcionalidades del código

Respone a la preguntas:
- ¿Puede el usuario hacer esto?
- ¿Funciona esta característica?

::right::

## Pruebas no funcionales

Pruebas que no están directamente relacionadas con las funcionalidades del sistema sino sus aspectos de calidad
como escalabilidad y rendimiento.

<!--
# Functional vs non-functional testing

- Functional testing refers to activities that verify a specific action or function of the code. These are usually found in the code requirements documentation, although some development methodologies work from use cases or user stories. Functional tests tend to answer the question of "can the user do this" or "does this particular feature work."

- Non-functional testing refers to aspects of the software that may not be related to a specific function or user action, such as scalability or other performance, behavior under certain constraints, or security. Testing will determine the breaking point, the point at which extremes of scalability or performance leads to unstable execution. Non-functional requirements tend to be those that reflect the quality of the product, particularly in the context of the suitability perspective of its users. 
-->

---
layout: image-right
image: ./assets/pyramid1.jpg
---
# Pruebas de sofware
## Niveles

Las pruebas de sofware se pueden categorizar en niveles dependiendo de cantidad del sistema que está siendo enfocado durante la prueba.

Las pruebas de sofware deberían tener un acercamiento "piramidal" donde la mayoría de los tests deberían ser tests unitarios,
seguido de los tests de integración y por último tests de punto a punto (E2E).

---

# Pruebas funcionales
## Pruebas unitarias

En este tipo de pruebas, se aisla una funcionalidad (unidad) para probar su funcionamiento y verificar que realice el comportamiento esperado.

Lo que se define como una unidad depende del paradigma y del enfoque:
- En programación procedural una unidad puede ser una función o módulo
- En programación orientada a objetos puede ser el método de una clase o una clase
  - Lo más común es hacer un test por cada método en una clase, a menos que los métodos de una clase estén muy acoplados

<!--
A unit is defined as a single behaviour exhibited by the system under test (SUT), usually corresponding to a requirement[definition needed]. While a unit may correspond to a single function or module (in procedural programming) or a single method or class (in object-oriented programming), functions/methods and modules/classes do not necessarily correspond to units. From the system requirements perspective only the perimeter of the system is relevant, thus only entry points to externally visible system behaviours define units.[clarification needed][10]
-->
---

# Pruebas funcionales
## Pruebas de aceptación

Una definición para este tipo de tests sería:
> Pruebas formales respecto a las necesides de un usuario, requrimientos y procesos de negocio,
> conducidas para determinar que un sistema satisface los criterios de aceptación.
>
> -- ISTQB

Suelen ser tests de "caja-negra": Se verifica la funcionalidad que se expone al usuario final.
Solo se sabe lo que el sistema debería hacer, no como lo hace

Un caso muy común es probar los endpoints de una API rest.

---

# Pruebas funcionales
## Pruebas de integración

En este tipo de pruebas, multiples partes de un sistema son evaluadas en conjunto.

Uno de los tests de integración más comunes es probar la integración de la base de datos con un componente.

---

# Pruebas funcionales
## Pruebas de regresión

Este tipo de pruebas hace referencia a volver a ejecutar tests funcionales y no funcionales para
asegurar que las funcionalidades desarrolladas anteriormente siguen funcionando correctamente
después de un cambio en el sistema. Si eso no sucede, se dice que ha ocurrido una "regresión"

Las técnicas para hacer tests de regresión son:

- Ejectuar todo el conjunto de pruebas
- Seleccionar un subconjunto de todas las pruebas
- Priorización de pruebas
  - General
  - Respecto a una versión particular
- Híbirido

<!--
# Test case prioritization

Prioritize the test cases so as to increase a test suite's rate of fault detection. Test case prioritization techniques schedule test cases so that the test cases that are higher in priority are executed before the test cases that have a lower priority.[9]
Types of test case prioritization

    - General prioritization – Prioritize test cases that will be beneficial on subsequent versions
    - Version-specific prioritization – Prioritize test cases with respect to a particular version of the software.
-->

---

# Pruebas no funcionales
## Pruebas de carga

Es el tests de rendimiento más simple. Usualmente se realiza para verificar el comportamiento de un sistema bajo una carga esperada.
Por ejemplo, el número de usuarios concurrentes esperados, realizando un número especifico de transacciones.

Sirve para ver los tiempos de respuesta que tendrá un sistema ante diferentes cargas.

<!--
Load testing is the simplest form of performance testing. A load test is usually conducted to understand the behavior of the system under a specific expected load. This load can be the expected concurrent number of users on the application performing a specific number of transactions within the set duration. This test will give out the response times of all the important business critical transactions. The database, application server, etc. are also monitored during the test, this will assist in identifying bottlenecks in the application software and the hardware that the software is installed on 
-->

---

# Pruebas no funcionales
## Pruebas de estres

Este tipo de pruebas se realiza para verificar los límites superiores de un sistema. Sirve para determinar si un sistema
funcionará lo suficientemente bien si la carga actual va más allá del máximo esperado.

<!--
Stress testing is normally used to understand the upper limits of capacity within the system. This kind of test is done to determine the system's robustness in terms of extreme load and helps application administrators to determine if the system will perform sufficiently if the current load goes well above the expected maximum. 
-->

---

# Pruebas no funcionales
## Pruebas de escalabilidad

Se conocen como pruebas de escalabilidad a aquellas pruebas no funcionales que permiten determinar el grado de escalabilidad que tiene un sistema. Se entiende como escalable la capacidad que tiene el sistema para que, sin aplicar cambios drásticos en su configuración, pueda soportar el incremento de demanda en la operación.

Un ejemplo de escalabilidad es si el sistema soporta la agregación de un nodo extra en su esquema de balanceo en la capa aplicativa o de base de datos, o un incremento en la memoria RAM o CPU´s en su infraestructura. 

---

# Pruebas no funcionales
## Pruebas de portabilidad

En este tipo de pruebas, se determina el grado de facilidad o dificultad que tiene un componente de software o aplicación
para transferirse efectiva y fáfilcmente desde un hardware, sotfware o ambiente operacional hacia otro.

<!--
Portability testing is the process of determining the degree of ease or difficulty to which a software component or application can be effectively and efficiently transferred from one hardware, software or other operational or usage environment to another.[1] The test results, defined by the individual needs of the system, are some measurement of how easily the component or application will be to integrate into the environment and these results will then be compared to the software system's non-functional requirement of portability[2] for correctness. The levels of correctness are usually measured by the cost to adapt the software to the new environment[3] compared to the cost of redevelopment.[4]
-->
