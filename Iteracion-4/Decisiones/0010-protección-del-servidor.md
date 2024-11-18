---
status: proposed
date: 18-11-2024
deciders: Daniel Santos López y Diego Sánchez Rincón
---

# 0010 Protección del servidor

* Status: proposed
* Date: 18-11-2024

## Context and Problem Statement

Con el fin de evitar ataques de denegación de servicio y saturar el servidor, el sistema otorgará al usuario de tipo cliente tres intentos a la hora de realizar un pedido para evitar errores.

## Decision Drivers

* **RF-05**: Permitir un máximo de tres peticiones al realizar un pedido

## Considered Options

* 0010-1 Patrón de diseño Circuit Breaker
* 0010-2 Patrón de diseño Retry + Circuit Breaker
* 0010-3 Patrón de diseño Retry

## Decision Outcome

**Chosen option**: 0010-2 Patrón de diseño Retry + Circuit Breaker, ***because*** con esta implementación se permite al usuario realizar tres intentos para realizar un pedido, mediante retry. Si el usuario supera los tres intentos, el sistema bloqueará las siguientes peticiones durante un tiempo determinado, utilizando circuit breaker.

### Consequences

* ***Good, because*** se permite al usuario realizar tres intentos para realizar un pedido. 
* ***Good, because*** se evitan ataques de denegación de servicio.
* ***Good, because*** se evita la saturación del servidor.
* ***Bad, because*** aumenta la complejidad del sistema.

## Pros and Cons of the Options

### 0010-1 Patrón de diseño Circuit Breaker

* ***Good, because*** se evitan ataques de denegación de servicio.
* ***Good, because*** se evita la saturación del servidor.
* ***Bad, because*** no se permite al usuario realizar tres intentos para realizar un pedido.

### 0010-2 Patrón de diseño Retry + Circuit Breaker

* ***Good, because*** se permite al usuario realizar tres intentos para realizar un pedido. 
* ***Good, because*** se evitan ataques de denegación de servicio.
* ***Good, because*** se evita la saturación del servidor.
* ***Bad, because*** aumenta la complejidad del sistema.

### 0010-3 Patrón de diseño Retry

* ***Good, because*** se permite al usuario realizar tres intentos para realizar un pedido.
* ***Bad, because*** necesita el Circuit Breaker para funcionar correctamente.
* ***Bad, because*** aumenta la complejidad del sistema.

## More Information

Para más información, se pueden consultar los siguientes recursos:

* [Retry](https://learn.microsoft.com/en-us/azure/architecture/patterns/retry)
* [Circuit Breaker](https://learn.microsoft.com/en-us/azure/architecture/patterns/circuit-breaker)