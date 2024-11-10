---
status: accepted
date: 09-11-2024
deciders: Daniel Santos López y Diego Sánchez Rincón
---

# 0004 Módulo de estadísticas

* Status: accepted
* Date: 09-11-2024

## Context and Problem Statement

El sistema deberá generar estadísticas automáticamente para los usuarios de tipo cliente acerca de los pedidos y la posición en tiempo real de los camiones. Para usuarios de tipo administrador también generará estadísticas acerca de los clientes.

## Decision Drivers

* **RF-11**: Mostrar estadísticas a los clientes
* **RF-12**: Mostrar estadísticas a los administradores

## Considered Options

* 0004-1 Microservicio de estadísticas
* 0004-2 Módulo de estadísticas en el sistema

## Decision Outcome

**Chosen option**: 0004-1 Microservicio de estadísticas, ***because*** permite desacoplar el módulo de estadísticas del resto del sistema y alojarlo en el docker remoto.

### Consequences

* ***Good, because*** permite desacoplar el módulo de estadísticas del resto del sistema.
* ***Good, because*** facilita el mantenimiento y la escalabilidad del sistema.
* ***Good, because*** permite desplegar y actualizar el módulo de estadísticas de forma independiente.
* ***Bad, because*** puede introducir complejidad adicional en la gestión de los microservicios.

## Pros and Cons of the Options

### 0004-1 Microservicio de estadísticas
* ***Good, because*** permite desacoplar el módulo de estadísticas del resto del sistema.
* ***Good, because*** facilita el mantenimiento y la escalabilidad del sistema.
* ***Good, because*** permite desplegar y actualizar el módulo de estadísticas de forma independiente.
* ***Bad, because*** puede introducir complejidad adicional en la gestión de los microservicios.

### 0004-2 Módulo de estadísticas en el sistema
* ***Good, because*** es más sencillo de implementar inicialmente.
* ***Good, because*** no requiere gestión adicional de microservicios.
* ***Bad, because*** acopla el módulo de estadísticas al resto del sistema, dificultando el mantenimiento y la escalabilidad.
* ***Bad, because*** las actualizaciones del módulo de estadísticas pueden afectar al resto del sistema.

## More Information

Para más información, se pueden consultar los siguientes recursos:

* [Microservicios](https://aws.amazon.com/es/microservices/#:~:text=Los%20microservicios%20son%20un%20enfoque,servicios%20son%20equipos%20peque%C3%B1os%20independientes.)
* [Docker](https://www.docker.com/)
* [Arquitectura de microservicios](https://martinfowler.com/articles/microservices.html)