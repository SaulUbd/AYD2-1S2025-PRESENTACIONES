---
theme: mint
title: Elementos de diseño
image: ./assets/ui_ux_cover.jpg
---

# Elementos de diseño
## y patrones de comportamiento
Análisis y Diseño de Sistemas 2
Saul Castellanos

---
layout: center
---

# Temas

- Patrones de comportamiento
- Repaso de estilos de arquitectura
- Elementos de diseño

---
layout: image-left
image: ./assets/observer.png
---

# Patrones de comportamiento
## [Observer](https://refactoring.guru/es/design-patterns/observer)

Observer es un patrón de diseño de comportamiento que te permite definir un mecanismo de suscripción para notificar a varios objetos sobre cualquier evento que le suceda al objeto que están observando.

El patrón Observer sugiere que añadas un mecanismo de suscripción a la clase notificadora para que los objetos individuales puedan suscribirse o cancelar su suscripción a un flujo de eventos que proviene de esa notificadora.

---
layout: image
backgroundSize: contain
image: ./assets/oberver-structure.png
---
---
layout: image-right
image: ./assets/strategy.png
---

# Patrones de comportamiento
## [Strategy](https://refactoring.guru/es/design-patterns/strategy)

Strategy es un patrón de diseño de comportamiento que te permite definir una familia de algoritmos, colocar cada uno de ellos en una clase separada y hacer sus objetos intercambiables.

El patrón Strategy sugiere que tomes una clase que hace algo específico de muchas formas diferentes y extraigas todos esos algoritmos para colocarlos en clases separadas llamadas estrategias.

---
layout: image
backgroundSize: contain
image: ./assets/strategy-structure.png
---
---
layout: image-left
image: ./assets/command-es.png
---

# Patrones de comportamiento
## [Command](https://refactoring.guru/es/design-patterns/command)

Command es un patrón de diseño de comportamiento que convierte una solicitud en un objeto independiente que contiene toda la información sobre la solicitud. Esta transformación te permite parametrizar los métodos con diferentes solicitudes, retrasar o poner en cola la ejecución de una solicitud y soportar operaciones que no se pueden realizar.

---
layout: image
backgroundSize: contain
image: ./assets/command-structure.png
---
---
layout: image-right
image: ./assets/iterator-es.png
---

# Patrones de comportamiento
## [Iterator](https://refactoring.guru/es/design-patterns/iterator)

Iterator es un patrón de diseño de comportamiento que te permite recorrer elementos de una colección sin exponer su representación subyacente (lista, pila, árbol, etc.).

La idea del patrón Iterator es extraer el comportamiento de recorrido de una colección y colocarlo en un objeto independiente llamado iterador.
Además de implementar el propio algoritmo, un objeto iterador encapsula todos los detalles del recorrido, como la posición actual y cuántos elementos quedan hasta el final.

---
layout: image
backgroundSize: contain
image: ./assets/iterator-structure.png
---
---
layout: image-left
image: ./assets/state-es.png
---

# Patrones de comportamiento
## [State](https://refactoring.guru/es/design-patterns/state)

State es un patrón de diseño de comportamiento que permite a un objeto alterar su comportamiento cuando su estado interno cambia. Parece como si el objeto cambiara su clase.

El patrón State sugiere que crees nuevas clases para todos los estados posibles de un objeto y extraigas todos los comportamientos específicos del estado para colocarlos dentro de esas clases.

---
layout: image
backgroundSize: contain
image: ./assets/state-structure-es.png
---
---
layout: two-cols-header
---

# Estilos de arquitectura
## _Estilos_ vs _Patrones_ (de arquitectura)

::left::

## Estilos de arquitectura

Se refire a la esctructura organizacional de alto nivel para un sistema de software.
Operan a un mayor nivel de abstracción que los patrones de arquitectura.

Definen cosas como:

- Como se organizan los componentes
- Como interactuan los componentes
- Que restricciones tienen dichas interacciones

::right::

## Patrones de arquitectura

Se refiere soluciones reusables a problemas recurrentes a **nivel de sistema**.
Operan a un mayor nivel de abstracción que los patrones de diseño.

Definen cosas como:

- Cualidades de calidad del sistema
- Estructura general del sistema

<!--
 Software Architecture Pattern refers to a reusable, proven solution to a recurring problem at the system level, addressing concerns related to the overall structure, component interactions, and quality attributes of the system. Software architecture patterns operate at a higher level of abstraction than software design patterns, solving broader system-level challenges. While these patterns typically affect system-level concerns, the distinction between architectural patterns and architectural styles can sometimes be blurry. Examples include Circuit Breaker. [1][2][3]

Software Architecture Style refers to a high-level structural organization that defines the overall system organization, specifying how components are organized, how they interact, and the constraints on those interactions. Architecture styles typically include a vocabulary of component and connector types, as well as semantic models for interpreting the system's properties. These styles represent the most coarse-grained level of system organization. Examples include Layered Architecture, Microservices, and Event-Driven Architecture. 
-->

---
layout: two-cols-header
---

# Estilos de arquitectura
[*fuente](https://en.wikipedia.org/wiki/List_of_software_architecture_styles_and_patterns)

::left::

**Estilos de arquitectura**
- Event-driven architecture
- Hexagonal Architecture (also known as Ports and Adapters)
- Layered architecture
    - Client–server model
- Microkernel architecture
- Pipes and Filters architecture
- Microservices
- Monolithic
- Service-oriented architecture
- Space-based architecture

::right::

**Patrones de arquitectura**
- Inbox and outbox pattern
- Asynchronous messaging
- Batch request
- Model–view–controller
- Peer-to-peer
- Publish–subscribe pattern
- Rate limiting
- Request–response
- Rule-based
- MVC

---
layout: image-right
image: ./assets/n-capas.png
---

# Estilos de arquitectura
## N-capas
[*fuente](https://en.wikipedia.org/wiki/Multitier_architecture)

Es un tipo de arquitectura donde las capas de presentación, lógica de negocio y de datos están separadas.
Se suele llamar n-layer o n-tier. **La aplicación más común de esta arquitectura es la de 3 capas.**

**Layer** hace referencia a la división conceptual de diferentes partes de un sistema.
**Tier** hace referencia a una división física para diferentes componentes de un sistema.
Una apliación de _N_ capas podría estar en un solo tier o _N_ tiers. Cabe recalcar que ambos terminos suelen usarse como sinonimos.

---

# Elementos de diseño
## Arquitectura de la información (IA)

IA es la disciplina de hacer la información fácil de encontrar y de entender. Incluye busqueda, navegación, categorización y presentación de información relevante e información contextual para ayudar a las personas a entender sus alrededores y a encontrar lo que están buscando, ya sea en la web o en el mundo real.

IA opera desde dos perspectivas:
- Las personas perciben información, productos y servicios como "lugares" hechos de _lenguaje_
- Estos "lugares" o "ambientes de información" pueden ser organizados para optimizar la buesqueda y el entendimiento de la información

_Lenguaje_ en este contexto significa elementos visuales, etiquetas, descripciones, menús y contenido. Podemos orgnanizar este "Lenguaje" para que todos estos elementos trabajen juntos para facilitar el entendimiento.

---
layout: image-left
image: ./assets/IA_diagram.png
---

# Elementos de diseño
## Arquitectura de la información

- Contenido
    - ¿Qué tipo de información está disponible?
    - ¿Qué relevancia tiene para el usuario?
- Contexto
    - ¿Donde está el usuario buscando el contenido?
    - ¿Cuándo, por qué y cómo está el usuario interactuando con el contenido?
- Usuario
    - ¿Quién está consumiendo el contenido?
    - ¿Qué valor provee?
    - ¿Qué espectativas preexistentes tienen?

<!--
La buena IA es informada por el contenido, contexto y usuarios
-->

---
layout: image
image: ./assets/information_architecture.jpg
backgroundSize: contain
---
---
layout: image-right
image: ./assets/ui_ux_1.jpg
---

# Elementos de diseño
## UI & UX
### UI (User Interface)

En el diseño digital, UI se refiere al a interactividad y apariencia de la pantalla de un producto o página web.

Hay 4 elementos clave a tomarse en cuenta:
- Diseño
- Paleta de colores y tipografía
- Elementos interactivos
- Fidelidad de maquetado y prototipado

<!--
To create engaging UI, designers consider these four key elements:

    - Page layout. Ideally, the organization of a web page or mobile app screen should seem intuitive to users. But to organize it that way, UI designers have to make dozens of well-considered decisions—from the header position to the amount of white space.
    - Color scheme and font selection. UI designers carefully choose the colors and fonts on a digital product interface for consistency, accessibility, and brand alignment.
    - Interactive elements. From button design to drop-down menus, UI designers style digital product screens to make user flows intuitive.
    - Wireframe and prototype fidelity. UX designers often put together basic wireframes and prototypes. UI designers can help transform them into high-fidelity, functional, interactive product mockups
-->

---
layout: image-right
image: ./assets/ui_ux_2.jpg
---

# Elementos de diseño
## UI & UX
### UX (User eXperience)

En el diseño digital, UX se refiere la experiencia en general que un usuario tiene con un producto o página web.

Hay 5 pasos esenciales para el diseño UX:

1. Investigación de consumidores y competencia
2. Arquitectura de la información
3. Maquetado y prototipos
4. Pruebas y resolución de problemas
5. Actualizaciones continuas

<!--
1. Consumer and competitor research

To deliver a positive user experience, UX designers need to understand their target audience. Through UX research, they discover what their users like, what problems and pain points they’re facing, and how they behave online or while using an app or software. UX designers may also perform competitor analysis using a SWOT analysis template to define their product niche.

UX designers often consolidate user research findings into buyer or user personas, which are detailed descriptions of target audience types.

2. Information architecture

Once UX designers understand users’ needs and behaviors, they can create information architecture (IA) for their product or site. Designers use IA as a visual blueprint, outlining essential navigation, content hierarchy, features, and interactions.

One key IA tool is a flowchart template, which designers use to map out key user flows and decision points. IA flowcharts help teams understand at a glance how the product is intended to work—and where there's a gap that may require additional features or updates.

3. Wireframes and prototypes

With IA sketched out, UX designers can start turning ideas into tangible models, such as wireframes and prototypes. Teams use these proofs of concept to test ideas, define requirements, and set feature priorities. Figma's online prototypes facilitate collaboration among designers, developers, and product owners, bringing everyone together to produce a more responsive, accessible, usable, and engaging end product.

4. Testing and troubleshooting

Product mockup tools created by Figma's community of professional designers help UX designers, developers, and product owners see how features will work in practice. If testing reveals issues like confusing navigation, menus, or forms, the team can adjust them before launch.

5. Ongoing updates

Even after a digital product has entered the market, a UX designer’s job is never truly done. With new user feedback and back-end analytics, they can design updates and improvements.For example, analytics may reveal that an e-commerce checkout process is too long, leading to a high cart abandonment rate. To address this issue, UX designers may streamline some checkout steps.
-->

---

# Elementos de diseño
## UI vs. UX

- UI se refiere a la interfaz directa con la que interactúan los usuarios en un software o sitio web, incluidos los elementos visuales y los controles. Es un subconjunto de UX, que es un término más amplio que abarca todos los puntos de contacto que un usuario tiene con un producto, incluido el servicio al cliente, la marca, los precios y más.
- Los términos UI y UX no deben utilizarse indistintamente, ya que tienen significados distintos. Un diseñador de UI es inherentemente un diseñador de UX, pero un diseñador de UX sin un campo de trabajo más específico es raro. Referirse a "UX" sin concretar puede hacer que una conversación carezca de sentido.

<!--
UI stands for User Interface. It’s what users interact with directly, everything they see, touch and hear within a piece of software or a website. It’s the outermost layer of an app – the controls.

In its current state – due to the types of devices we are using – UI design is mostly a visual discipline, although voice and written word are gaining more and more traction thanks to voice assistants and conversational interfaces.

UX stands for User eXperience. It’s a holistic term encapsulating each and every different kind of touchpoint a user has with a product.

In the context of a digital product, this includes not only the software’s front-end itself, but the whole technical stack, customer service, branding, public image of the company, availability, pricing, and communication, and that’s certainly not all.

UI is a subset of UX. Both terms have different meanings and, whenever possible, should not be used interchangeably. The title “UX/UI designer” makes little sense in terms of semantics. Every UI designer is a UX designer by definition, and being a UX designer without a more specific field of work is quite rare. Talking about “UX” without specifics can quickly render any conversation meaningless.
-->

