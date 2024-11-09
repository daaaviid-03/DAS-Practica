---
status: accepted
date: 09-11-2024
deciders: Daniel Santos López y Diego Sánchez Rincón
---

# 0004 Módulo de estadísitcas

* Status: accepted
* Date: 09-11-2024

## Context and Problem Statement

El sistema deberá generar estadisticas automáticamente para los usuarios de tipo cliente acerca de los pedidos y la posición en tiempo real de los camiones. Para usuarios de tipo administrtador también generará estadisticas acerca de los clientes.


## Decision Drivers

* **RF-11**: Mostrar estadisticas a los clientes
* **RF-12**: Mostrar estadisticas a los administradores

## Considered Options

* 0004-1 Microservicio de estadísitcas

## Decision Outcome

**Chosen option**: 0004-1 Microservicio de estadísitcas, ***because*** permite desacoplar el módulo de estadísitcas del resto del sistema y alojarlo en el docker remoto.

### Consequences

* ***Good, because*** permite la flexibilidad de cambiar entre diferentes algoritmos de optimización.
* ***Good, because*** desacopla el algoritmo del resto del sistema, lo que facilita su gestión y mantenimiento.
* ***Good, because*** permite una clara separación de responsabilidades
* ***Bad, because*** pueden añadir complejidad al sistema.

## More Information

Para más información, se pueden consultar los siguientes recursos:

* [Strategy pattern](https://refactoring.guru/design-patterns/strategy)

