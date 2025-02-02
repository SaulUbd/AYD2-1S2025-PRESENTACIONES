---
title: "Frameworks y patrones de Diseño"
theme: seriph
---

# Frameworks y patrones de diseño
Análisis y Diseño de Sistemas 2

---
layout: center
---

# Agenda
1. Lectura del programa
2. Creacion de grupos
3. Presentacion
4. Ejemplo practico

---

# Frameworks
## ¿Qué es un framework?
En programación un framework es una abstracción en la que el software, que proporciona una funcionalidad genérica,
puede modificarse selectivamente mediante código adicional escrito por el usuario,
proporcionando así un software específico para la aplicación.

<!--
In computer programming, a software framework is an abstraction in which software, providing generic functionality, can be selectively changed by additional user-written code, thus providing application-specific software. It provides a standard way to build and deploy applications and is a universal, reusable software environment that provides particular functionality as part of a larger software platform to facilitate the development of software applications, products and solutions.

Software frameworks may include support programs, compilers, code libraries, toolsets, and application programming interfaces (APIs) that bring together all the different components to enable development of a project or system. 
-->
---

# Características

- Inversion de control
- Comportamiento por defecto
- Extensibilidad
- Codigo no modificable

Cada framework implementa algún patrón de arquitectura, y expone APIs o funcionalidades que permiten
la extensibilidad del software que se desarrolla. El software desarrollado a través de un framework
termina siguiendo el mismo patrón de arquitectura en alta o baja medida.

<!--
inversion of control: In a framework, unlike in libraries or in standard user applications, the overall program's flow of control is not dictated by the caller, but by the framework.[1] This is usually achieved with the Template Method Pattern.
default behaviour: This can be provided with the invariant methods of the Template Method Pattern in an abstract class which is provided by the framework.
extensibility: A user can extend the framework–usually by selective overriding–or programmers can add specialized user code to provide specific functionality. This is usually achieved by a hook method in a subclass that overrides a template method in the superclass.
non-modifiable framework code: The framework code, in general, is not supposed to be modified, while accepting user-implemented extensions. In other words, users can extend the framework, but cannot modify its code.

Es decir, algunos frameworks te obligan a seguir algún patrón de arquitectura, mientras que otros son más libres o permisivos
-->

---
layout: section
---

# Tipos de Frameworks

---

# 1. Frameworks Frontend
Estos son frameworks enfocados a la presentación

- Spring MVC
- Angular
- Nuxt
- Astro

---

# 2. Frameworks Backend
Estos son frameworks enfocados en la lógica de negocio

- Spring Boot
- Express
- FastApi

---

# 3. Frameworks Fullstack
Estos son frameworks que pueden ser usados tanto para frontend como backend.
Suelen tener todo lo necesario para hacer aplicaciones fullstack,
es decir, presentación y lógica de negocio en un mismo paquete, con una
misma base de código.

- Laravel
- Sveltekit
- ASP.NET Core

---

# 4. Frameworks de Desarrollo Móvil
- Flutter
- React Native
- SwiftUI

---

# 5. Frameworks de Desarrollo de Juegos
- Unity
- Unreal Engine
- Godot Engine

---
layout: section
---

# Frameworks Vs. librerías
[Video explicativo](https://youtu.be/A-iKX8Shge4?si=u4RnJomNCPn2L7ME)

---
layout: image
image: ./assets/framework_vs_lib.jpg
backgroundSize: contain
---

---
layout: section
---

# Patrones de diseño
## Estilos arquitectonics, patrones de arquitectura, patrones de diseño

<!--
Es muy común escuchar cosas como MVC, Arquitectura por capas, arquitectura basada en eventos, etc.
¿Pero exactamente cómo se categoriza cada cosa?
Vamos a trabajar con 3 conceptos
-->
---

# Estilos arquitectonicos
Son enfoques generales que dictan cómo se estructura y organiza un sistema de software.
Representan principios de diseño a gran escala y establecen reglas para la interacción entre los componentes.

- Cliente-Servidor
- Microservicios
- Monolítico
- Arquitectura en capas
- Architecture orienta a eventos

---

# Patrones de arquitectura

Son soluciones reutilizables y bien definidas para problemas comunes dentro de una arquitectura de software. Son más específicos que los estilos arquitectónicos y pueden implementarse dentro de ellos.

- MVC (Modelo-Vista-Controlador)
- Pub-sub
- Broker

---

# Patrones de diseño

Son soluciones reutilizables a problemas recurrentes en la implementación del código.
Se aplican a nivel de desarrollo y organización del código dentro de una arquitectura.

- Singleton
- Factory Method
- Observer
- Adapter
- Decorator
- Inversion de dependencias

---

# Resumen

Son niveles de especificación para describir la implementación de un sistema de software.

- Los estilos arquitectonicos definen la forma de un sistema y reglas de interacion entre los componentes
de un sistema de software
- Los patrones de arquitectura son formas en que implementamos estilos de arquitectura o problemas
comunes al desarrollar un sistema de sofware
- Los patrones de diseño son formas en que implementamos patrones de arquitectura o problemas
comunes al desarrollar funcionalidades

Y si fueramos más profundo, llegaríamos a los paradigmas de programación (Orientado a objetos, funcional, imperativo, declarativo, etc.)

---
layout: end
---

# Gracias 😊
