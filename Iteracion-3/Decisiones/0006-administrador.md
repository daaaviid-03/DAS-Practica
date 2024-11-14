---
status: accepted
date: 14-11-2024
deciders: David Pimentel y Marcos García
---

# 0006 Incluir un usuario administrador

* Status: accepted
* Date: 14-11-2024

## Context and Problem Statement

Se necesita un usuario administrador capaz de modificar en tiempo de ejecución aspectos como los productos ofertados (añadiendo, eliminando o modificando productos) o gestionar las flotas de camiones dando de alta o de baja camiones y repartidores.

## Decision Drivers

* **RF-15**: Gestionar y modificar pedidos

## Considered Options

* 0006-1 Crear un rol de usuario administrador con permisos específicos
* 0006-2 Implementar un sistema interno dedicado a la administración

## Decision Outcome

**Chosen option**: 0006-1 Crear un rol de usuario administrador con permisos específicos, ***because*** permitirá una gestión segura y sencilla, con control directo de los permisos dentro del sistema, sin necesidad de implementar un módulo del sistema totalmente dedicado a la gestión realizada por los administradores como propone la opción 0006-2.

### Consequences

* ***Good, because*** establece un control sencillo de los permisos.
* ***Good, because*** permite asignar responsabilidades administrativas de forma segura y estructurada.
* ***Good, because*** permite una clara separación de responsabilidades entre usuarios.
* ***Bad, because*** puede agregar complejidad adicional en términos de desarrollo y pruebas.

## Pros and Cons of the Options

### 0006-1 Crear un rol de usuario administrador con permisos específicos

* ***Good, because*** permite un control directo sobre la administración de permisos.
* ***Good, because*** es fácil de escalar y ajustar según los cambios en las funciones administrativas.
* ***Good, because*** seguridad mejorada, al limitar el acceso solo a funciones necesarias.
* ***Bad, because*** aumento en la realización de pruebas y controles de seguridad, para controlar los permisos de los administradores.

### 0006-2 Implementar un sistema interno dedicado a la administración

* ***Good, because*** permite una personalización máxima para adaptarse a necesidades específicas al ser un sistema dedicado.
* ***Bad, because*** mayor riesgo de errores de seguridad si no se implementa cuidadosamente.
* ***Bad, because*** incremento en la carga de desarrollo y mantenimiento del sistema de administración.

## More Information

Para más información, se pueden consultar los siguientes recursos:

* [Principle of Least Privilege](https://www.paloaltonetworks.com/cyberpedia/what-is-the-principle-of-least-privilege)
