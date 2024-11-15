---
status: accepted
date: 15/11/2024
deciders: Daniel Santos López y Diego Sánchez Rincón
---

# 0008 Módulo de pedidos

* Status: accepted
* Date: 15/11/2024

## Context and Problem Statement

El sistema debe permitir a los usuarios de tipo cliente realizar pedidos de los productos disponibles. Para ello, se necesita un módulo que permita gestionar los pedidos de los clientes.

## Decision Drivers

* **RF-04**: Realizar pedidos
* **RF-06**: Procesar pedidos

## Considered Options

* 0008-1 Implementar el módulo de pedidos como un microservicio independiente
* 0008-2 Integrar el módulo de pedidos dentro del sistema existente

## Decision Outcome

**Chosen option**: 0008-2 Integrar el módulo de pedidos dentro del sistema existente, ***because*** los pedidos son la parte más crítica del sistema y no es recomendable depender de un microservicio para ello.

### Consequences

* ***Good, because*** asegura que la funcionalidad crítica de pedidos esté siempre disponible y no dependa de la comunicación entre microservicios.
* ***Good, because*** simplifica la implementación inicial y la gestión del sistema.
* ***Good, because*** facilita la integración con el resto de los módulos del sistema.
* ***Bad, because*** las actualizaciones del módulo de pedidos pueden afectar al resto del sistema.

## Pros and Cons of the Options

### 0008-1 Implementar el módulo de pedidos como un microservicio independiente
* ***Good, because*** permite una mayor modularidad y escalabilidad del sistema.
* ***Good, because*** facilita el mantenimiento y la actualización del módulo de pedidos de forma independiente.
* ***Bad, because*** puede introducir complejidad adicional en la gestión de los microservicios.
* ***Bad, because*** los pedidos son la parte más crítica del sistema y no es recomendable depender de un microservicio para ello.

### 0008-2 Integrar el módulo de pedidos dentro del sistema existente
* ***Good, because*** asegura que la funcionalidad crítica de pedidos esté siempre disponible y no dependa de la comunicación entre microservicios.
* ***Good, because*** simplifica la implementación inicial y la gestión del sistema.
* ***Good, because*** facilita la integración con el resto de los módulos del sistema.
* ***Bad, because*** las actualizaciones del módulo de pedidos pueden afectar al resto del sistema.

## More Information

* [Microservicios](https://aws.amazon.com/es/microservices/#:~:text=Los%20microservicios%20son%20un%20enfoque,servicios%20son%20equipos%20peque%C3%B1os%20independientes.)
* [Docker](https://www.docker.com/)