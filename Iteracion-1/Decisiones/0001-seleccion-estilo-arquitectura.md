---
status: accepted
date: 2024-11-02
deciders: David Pimentel, Marcos García, Daniel Santos, Diego Sánchez, Cristian Teijeiro y Juan Manuel Bustos
---

# 0001 Selección del Estilo de la Arquitectura Software

* Status: accepted
* Date: 2024-11-02

## Context and Problem Statement

Se necesita una arquitectura de software para crear una aplicación de gestión de pedidos y rutas de flotas de camiones.

## Decision Drivers

* **RF-01**: Acceso a datos del Cliente
* **RF-06**: Realizar pedidos
* **RF-09**: Gestión de flotas
* **RF-11**: Proveer datos sobre el estado de los pedidos

## Considered Options

* 0001-1 Arquitectura Cliente Servidor
* 0001-2 Modelo Vista Controlador
* 0001-3 Event Driven

## Decision Outcome

**Chosen option**: 0001-1 Arquitectura Cliente Servidor, ***because*** es el estilo arquitectónico que más se adapta al problema que se nos presenta debido a la estructura de las consultas del cliente al servidor. Además, es fácil de implementar y mantener, y permite una clara separación de responsabilidades.

### Consequences

* ***Good, because*** respalda la estructura de las colsultas de los clientes al servidor
* ***Good, because*** es fácil de implementar y mantener
* ***Good, because*** permite una clara separación de responsabilidades
* ***Bad, because*** puede tener problemas de escalabilidad en sistemas muy grandes
* ***Bad, because*** no es el estilo arquitectónico más moderno

## Pros and Cons of the Options

### 0001-1 Arquitectura Cliente Servidor

* ***Good, because*** permite una comunicación directa entre el cliente y el servidor
* ***Good, because*** es una arquitectura bien conocida y documentada
* ***Good, because*** es fácil de implementar y mantener
* ***Neutral, because*** puede requerir una gestión cuidadosa de la carga del servidor
* ***Bad, because*** puede ser menos eficiente en términos de rendimiento en comparación con arquitecturas más modernas

### 0001-2 Modelo Vista Controlador

* ***Good, because*** separa claramente la lógica de negocio de la presentación
* ***Good, because*** facilita el mantenimiento y la escalabilidad del código
* ***Neutral, because*** puede requerir más esfuerzo inicial en la configuración
* ***Bad, because*** puede ser más difícil de depurar debido a la separación de componentes
* ***Bad, because*** puede ser excesivo para aplicaciones simples

### 0001-3 Event Driven

* ***Good, because*** es adecuado para aplicaciones que requieren procesamiento en tiempo real
* ***Neutral, because*** puede ser más complejo de implementar y depurar
* ***Bad, because*** puede introducir latencia en la comunicación entre componentes
* ***Bad, because*** puede ser más difícil de mantener y escalar en comparación con otros estilos arquitectónicos

## More Information

Para más información, se pueden consultar los siguientes recursos:

* [Arquitectura Cliente Servidor](https://es.wikipedia.org/wiki/Arquitectura_cliente-servidor)
* [Modelo Vista Controlador](https://es.wikipedia.org/wiki/Modelo%E2%80%93vista%E2%80%93controlador)
* [Arquitectura Event Driven](https://es.wikipedia.org/wiki/Arquitectura_dirigida_por_eventos)