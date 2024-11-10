---
status: accepted
date: 10-11-2024
deciders: Daniel Santos López y Diego Sánchez Rincón
---

# 0005 Base de datos

* Status: accepted
* Date: 10-11-2024

## Context and Problem Statement

El sistema deberá almacenar los datos de los clientes y los pedidos en una base de datos para poder ser consultados en cualquier momento.
Los datos de los clientes se relacionan con los pedidos para poder identificar a qué cliente pertenece cada pedido.

## Decision Drivers

* **RF-17**: Acceso a BBDD

## Considered Options

* 0005-1 Base de datos relacional (MySQL)
* 0005-2 Base de datos relacional (PostgreSQL)
* 0005-3 Base de datos no relacional (MongoDB)

## Decision Outcome

**Chosen option**: 0005-2 Base de datos relacional (PostgreSQL), ***because*** almacena los datos de forma estructurada y permite la escalabilidad de la base de datos en caso de que el sistema crezca, ofreciendo un mejor rendimiento que MySQL en operaciones complejas.

### Consequences

* ***Good, because*** almacena los datos de forma estructurada
* ***Good, because*** permite la escalabilidad de la base de datos en caso de que el sistema crezca
* ***Good, because*** ofrece un mejor rendimiento que MySQL en operaciones complejas
* ***Bad, because*** requiere de un mayor esfuerzo en la configuración inicial

## Pros and Cons of the Options

### 0005-1 Base de datos relacional (MySQL)

* ***Good, because*** es una base de datos relacional
* ***Good, because*** es una base de datos ampliamente utilizada
* ***Bad, because*** no ofrece un buen rendimiento en operaciones complejas
* ***Bad, because*** no es tan escalable como PostgreSQL

### 0005-2 Base de datos relacional (PostgreSQL)

* ***Good, because*** almacena los datos de forma estructurada
* ***Good, because*** permite la escalabilidad de la base de datos en caso de que el sistema crezca
* ***Good, because*** ofrece un mejor rendimiento que MySQL en operaciones complejas
* ***Bad, because*** requiere de un mayor esfuerzo en la configuración inicial

### 0005-3 Base de datos no relacional (MongoDB)

* ***Good, because*** es una base de datos ampliamente utilizada
* ***Good, because*** es fácil de implementar
* ***Bad, because*** no almacena los datos de forma estructurada
* ***Bad, because*** no ofrece un buen rendimiento en operaciones complejas
* ***Bad, because*** no es tan escalable como PostgreSQL

## More Information

Para más información se pueden consultar los siguientes recursos:

* [PostgreSQL](https://www.postgresql.org/)
* [MySQL](https://www.mysql.com/)
* [MongoDB](https://www.mongodb.com/)
* [Diferencias entre PostgreSQL y MySQL](https://www.digitalocean.com/community/tutorials/sqlite-vs-mysql-vs-postgresql-a-comparison-of-relational-database-management-systems)