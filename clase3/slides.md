---
theme: mint
title: Patrones de Diseño - parte 2
image: ./assets/meme.jpg
---

# Patrones de Diseño
## Creacionales y Estructurales
Análisis y Diseño de Sistemas 2
Saul Castellanos

---
layout: image-left
image: ./assets/factory-method-es.png
---

# Patrones Creacionales
## [Factory method](https://refactoring.guru/es/design-patterns/factory-method)

El patrón Factory Method sugiere que, en lugar de llamar al operador `new` para construir objetos directamente, se invoque a un método fábrica especial. Los objetos se siguen creando a través del operador `new`, pero se invocan desde el método fábrica. Los objetos devueltos por el método fábrica a menudo se denominan productos.

---
layout: image
image: ./assets/factory-method-structure.png
backgroundSize: contain
---

---
layout: image-right
image: ./assets/abstract-factory-es.png
---

# Patrones Creacionales
## [Abstract factory](https://refactoring.guru/es/design-patterns/abstract-factory)

Abstract Factory es un patrón de diseño creacional que nos permite producir familias de objetos relacionados sin especificar sus clases concretas.

Consiste en declarar una Fábrica abstracta: una interfaz con una lista de métodos de creación para todos los productos que son parte de la familia de productos (por ejemplo, crearSilla, crearSofá y crearMesilla). Estos métodos deben devolver productos abstractos representados por las interfaces como: Silla, Sofá, Mesilla, etc.

---
layout: image
image: ./assets/abstract-factory-structure.png
backgroundSize: contain
---
---
layout: image-left
image: ./assets/singleton.png
---
# Patrones Creacionales
## [Singleton](https://refactoring.guru/es/design-patterns/singleton)

Singleton es un patrón de diseño creacional que nos permite asegurarnos de que una clase tenga una única instancia, a la vez que proporciona un punto de acceso global a dicha instancia.

Todas las implementaciones del patrón Singleton tienen estos dos características en común:
- Hacer privado el constructor por defecto
- Crear un método de creación estático que actúe como constructor

<!--
Todas las implementaciones del patrón Singleton tienen estos dos pasos en común:
- Hacer privado el constructor por defecto para evitar que otros objetos utilicen el operador `new` con la clase Singleton.
- Crear un método de creación estático que actúe como constructor. Tras bambalinas, este método invoca al constructor privado para crear un objeto y lo guarda en un campo estático. Las siguientes llamadas a este método devuelven el objeto almacenado en caché.

Si tu código tiene acceso a la clase Singleton, podrá invocar su método estático. De esta manera, cada vez que se invoque este método, siempre se devolverá el mismo objeto.
-->

---
layout: image
image: ./assets/singleton-structure-es.png
backgroundSize: contain
---
---
layout: image-right
image: ./assets/adapter-es.png
---
# Patrones Estructurales
## [Adapter](https://refactoring.guru/es/design-patterns/adapter)

Adapter es un patrón de diseño estructural que permite la colaboración entre objetos con interfaces incompatibles.

Un adaptador envuelve uno de los objetos para esconder la complejidad de la conversión que tiene lugar tras bambalinas. El objeto envuelto ni siquiera es consciente de la existencia del adaptador. Por ejemplo, puedes envolver un objeto que opera con metros y kilómetros con un adaptador que convierte todos los datos al sistema anglosajón, es decir, pies y millas.

---
layout: image
image: ./assets/structure-object-adapter.png
backgroundSize: contain
---
---
layout: image-left
image: ./assets/decorator.png
---
# Patrones Estructurales
## [Decorator](https://refactoring.guru/es/design-patterns/decorator)

Decorator es un patrón de diseño estructural que te permite añadir funcionalidades a objetos colocando estos objetos dentro de objetos encapsuladores especiales que contienen estas funcionalidades.

“Wrapper” (envoltorio, en inglés) es el sobrenombre alternativo del patrón Decorator, que expresa claramente su idea principal. Un wrapper es un objeto que puede vincularse con un objeto objetivo. El wrapper contiene el mismo grupo de métodos que el objetivo y le delega todas las solicitudes que recibe. No obstante, el wrapper puede alterar el resultado haciendo algo antes o después de pasar la solicitud al objetivo.

---
layout: image
image: ./assets/decorator-structure.png
backgroundSize: contain
---
---
layout: image-right
image: ./assets/facade.png
---
# Patrones Estructurales
## [Facade](https://refactoring.guru/es/design-patterns/facade)

Facade es un patrón de diseño estructural que proporciona una interfaz simplificada a una biblioteca, un framework o cualquier otro grupo complejo de clases.

Una fachada es una clase que proporciona una interfaz simple a un subsistema complejo que contiene muchas partes móviles. Una fachada puede proporcionar una funcionalidad limitada en comparación con trabajar directamente con el subsistema. Sin embargo, tan solo incluye las funciones realmente importantes para los clientes.

---
layout: image
image: ./assets/facade-structure.png
backgroundSize: contain
---
---
layout: image-left
image: ./assets/proxy.png
---
# Patrones Estructurales
## [Proxy](https://refactoring.guru/es/design-patterns/proxy)

Proxy es un patrón de diseño estructural que te permite proporcionar un sustituto o marcador de posición para otro objeto. Un proxy controla el acceso al objeto original, permitiéndote hacer algo antes o después de que la solicitud llegue al objeto original.

El patrón Proxy sugiere que crees una nueva clase proxy con la misma interfaz que un objeto de servicio original. Después actualizas tu aplicación para que pase el objeto proxy a todos los clientes del objeto original. Al recibir una solicitud de un cliente, el proxy crea un objeto de servicio real y le delega todo el trabajo.

---
layout: image
image: ./assets/proxy-structure.png
backgroundSize: contain
---
