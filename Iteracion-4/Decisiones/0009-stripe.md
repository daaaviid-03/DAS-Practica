---
status: proposed
date: 18-11-2024
deciders: Diego Sánchez Rincón y Daniel Santos López
---

# 0009 Stripe

* Status: proposed
* Date: 18-11-2024

## Context and Problem Statement

El sistema se conectará con la pasarela de pago de Stripe para procesar los pagos de los pedidos realizados por parte de los clientes. Esto garantizará la seguridad de los pagos.

## Decision Drivers

* **RF-14**: Gestionar pagos con una pasarela externa

## Considered Options

* 0009-1 Stripe

## Decision Outcome

**Chosen option**: 0009-1 Stripe, ***because*** permite gestionar los pagos de forma segura y eficiente. Es una pasarela de pago ampliamente utilizada y con una buena reputación. Además, es una imposición del cliente.

### Consequences

* ***Good, because*** permite gestionar los pagos de forma segura y eficiente.
* ***Good, because*** es una pasarela de pago ampliamente utilizada y con una buena reputación.
* ***Good, because*** el cliente lo ha impuesto como requisito.
* ***Bad, because*** aumenta la complejidad del sistema.

## Pros and Cons of the Options

### 0009-1 Stripe

* ***Good, because*** permite gestionar los pagos de forma segura y eficiente.
* ***Good, because*** es una pasarela de pago ampliamente utilizada y con una buena reputación.
* ***Good, because*** el cliente lo ha impuesto como requisito.
* ***Bad, because*** aumenta la complejidad del sistema.

## More Information

* [Stripe](https://stripe.com/)