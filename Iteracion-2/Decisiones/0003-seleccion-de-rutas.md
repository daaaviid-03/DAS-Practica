---
status: accepted
date: 09-11-2024
deciders: David Pimentel y Marcos García
---

# 0003 Selección de rutas

* Status: accepted
* Date: 09-11-2024

## Context and Problem Statement

La nueva arquitectura debe ser capaz de seleccionar el algoritmo óptimo para la optimización de rutas en función del retraso del camión.

## Decision Drivers

* **RF-08**: Selección de algoritmo de optimización

## Considered Options

* 0003-1 Strategy pattern

## Decision Outcome

**Chosen option**: 0003-1 Strategy pattern, ***because*** permite desacoplar el algoritmo de optimización de rutas del resto del sistema, facilitando el cambio entre diferentes algoritmos de optimización.

### Consequences

* ***Good, because*** permite la flexibilidad de cambiar entre diferentes algoritmos de optimización.
* ***Good, because*** desacopla el algoritmo del resto del sistema, lo que facilita su gestión y mantenimiento.
* ***Good, because*** permite una clara separación de responsabilidades
* ***Bad, because*** pueden añadir complejidad al sistema.

## More Information

Para más información, se pueden consultar los siguientes recursos:

* [Strategy pattern](https://refactoring.guru/design-patterns/strategy)

