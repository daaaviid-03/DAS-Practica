---
status: accepted
date: 14-11-2024
deciders: Daniel Santos López y Diego Sánchez Rincón
---

# 0007 Módulo de incidencias

* Status: accepted
* Date: 14-11-2024

## Context and Problem Statement

El sistema deberá permitir reportar a los gestores de las rutas cualquier tipo de incidencia (camión averiado, reparto no realizado, etc.). Este módulo es semi crítico ya que afecta directamente a la eficiencia y efectividad de las operaciones diarias.

## Decision Drivers

* **RF-16**: Gestionar incidencias en el reparto

## Considered Options

* 0008-1 Microservicio de incidencias
* 0008-2 Módulo de incidencias dentro de la lógica de negocio

## Decision Outcome

**Chosen option**: 0008-1 Microservicio de incidencias, ***because*** permite desacoplar el módulo de incidencias del resto del sistema, facilitando su mantenimiento y escalabilidad.

### Consequences

* ***Good, because*** permite desacoplar el módulo de incidencias del resto del sistema, facilitando su mantenimiento y escalabilidad.
* ***Good, because*** facilita la integración con otros sistemas.
* ***Good, because*** permite una mayor flexibilidad en el desarrollo.
* ***Bad, because*** aumenta la complejidad del sistema.

## Pros and Cons of the Options

### 0008-1 Microservicio de incidencias

* ***Good, because*** permite desacoplar el módulo de incidencias del resto del sistema, facilitando su mantenimiento y escalabilidad.
* ***Good, because*** facilita la integración con otros sistemas.
* ***Good, because*** permite una mayor flexibilidad en el desarrollo.
* ***Bad, because*** aumenta la complejidad del sistema.

### 0008-2 Módulo de incidencias dentro de la lógica de negocio

* ***Good, because*** reduce la complejidad del sistema.
* ***Bad, because*** dificulta la integración con otros sistemas.
* ***Bad, because*** dificulta el mantenimiento y escalabilidad del sistema.
* ***Bad, because*** reduce la flexibilidad en el desarrollo.

## More Information

Para más información, se pueden consultar los siguientes recursos:

* [Microservicios](https://aws.amazon.com/es/microservices/#:~:text=Los%20microservicios%20son%20un%20enfoque,servicios%20son%20equipos%20peque%C3%B1os%20independientes.)
* [Docker](https://www.docker.com/)
* [Arquitectura de microservicios](https://martinfowler.com/articles/microservices.html)