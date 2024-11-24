---
status: accepted
date: 19-11-2024
deciders: Marcos García y David Pimentel
---

# 0011 Procesado de pedidos

* Status: accepted
* Date: 19-11-2024

## Context and Problem Statement

El sistema de pedidos debe pasar siempre por una cadena de tres fases: preprocesado, autorización y aceptación, de manera que no es posible pasar a un estado si no es procesado correctamente el estado anterior. 

## Decision Drivers

* **RF-06**: Procesar pedidos

## Considered Options

* 0011-1 Patrón Chain of Responsibility
* 0011-2 Utilizar un enumerado con los estados

## Decision Outcome

**Chosen option**: 0011-1 Patrón Chain of Responsibility, ***because*** esta implementación permite controlar que el pedido pase siempre por todos los estados en un orden determinado y evita que el pedido pase a un estado sin haber sido procesado correctamente el estado anterior.

### Consequences

* ***Good, because*** se controla que el pedido pase siempre por todos los estados en un orden determinado.
* ***Good, because*** se evita que el pedido pase a un estado sin haber sido procesado correctamente el estado anterior.
* ***Bad, because*** aumenta la complejidad del sistema.

## Pros and Cons of the Options

### 0011-1 Patrón Chain of Responsibility

* ***Good, because*** se controla que el pedido pase siempre por todos los estados en un orden determinado.
* ***Good, because*** se evita que el pedido pase a un estado sin haber sido procesado correctamente el estado anterior.
* ***Bad, because*** aumenta la complejidad del sistema.

### 0011-2 Utilizar un enumerado con los estados

* ***Good, because*** es una solución más sencilla.
* ***Bad, because*** no se controla que el pedido pase siempre por todos los estados en un orden determinado.
* ***Bad, because*** se puede pasar a un estado sin haber sido procesado correctamente el estado anterior.

## More Information

Para más información, se pueden consultar los siguientes recursos:

* [Chain of Responsibility](https://refactoring.guru/design-patterns/chain-of-responsibility)