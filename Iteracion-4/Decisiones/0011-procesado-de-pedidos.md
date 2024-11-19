---
status: proposed
date: 19-11-2024
deciders: Marcos García y David Pimentel
---

# 0011 Procesado de pedidos

* Status: proposed
* Date: 19-11-2024

## Context and Problem Statement

El sistema de pedidos debe pasar siempre por una cadena de tres fases: preprocesado, autorización y aceptación, de manera que no es posible pasar a un estado sino se procesado correctamente el estado anterior. 

## Decision Drivers

* **RF-06**: Procesar pedidos

## Considered Options

* 0011-1 Patrón Chain of Responsibility
* 0011-2 Utilizar un enumerado con los estados

## Decision Outcome

**Chosen option**: 0011-1 Patrón Chain of Responsibility, ***because*** esta implementación permite controlar que el pedido pase siempre por todos los estados en un orden determinado

### Consequences

** Completar

## Pros and Cons of the Options
** Completar

## More Information
** Completar