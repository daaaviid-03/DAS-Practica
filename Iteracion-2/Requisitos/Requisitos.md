# Requisitos Funcionales

## **RF-01**: Pasar de arquitectura monolítica a una de microservicios 
> El sistema deberá de pasar de una arquitectura monolítica a una de microservicios para poder tener una mayor modularidad.

## **RF-02**: Conexión cliente-servidor
> 

## **RF-03**: Acceso a datos del Cliente
> El sistema permitirá al usuario de tipo cliente acceder a su información personal para poder añadir, modificar o eliminar esa información.

## **RF-04**: Realizar pedidos
> El sistema permitirá al usuario de tipo cliente realizar pedidos de los productos disponibles.

## **RF-05**: Permitir un máximo de tres peticiones al realizar un pedido
> El sistema otorgará al usuario de tipo cliente tres intentos a la hora de realizar un pedido para evitar errores.

## **RF-06**: Procesar pedidos 
> Cada pedido deberá pasa por tres fases secuenciales (preprocesado, autorización, y aceptación) y no puede avanzar a la siguiente fase sin haber completado la anterior. De esta forma se asegura la validez de los pedidos.

## **RF-07**: Gestión de flotas
> El sistema permitirá al usuario de tipo Administrador añadir, modificar o eliminar los camiones de las flotas.

## **RF-08**: Selección de algoritmo de optimización
> El sistema podrá legir entre dos algoritmos de optimización de rutas. Se debe utilizar uno u otro según la demora del camión.

## **RF-09**: Proveer datos sobre el estado de los pedidos
> El sistema deberá mantener actualizado el estado de los pedidos para que los clientes puedan consultarlo y saber el progreso de su pedido.

## **RF-10**: Recibir la posición de los camiones
> El sistema registrará mediante señal GPS la posición de los camiones en tiempo real, almacenándola para que esta sea accesible en cualquier momento.

## **RF-11**: Mostrar estadisticas de los clientes


## **RF-12**: Reportar incidencia
> El sistema permitirá al usuario de tipo repartidor reportar incidencias en tiempo real para registrarlas en el sistema.

## **RF-13**: Gestionar pagos con una pasarela externa
> El sistema se conectará con la pasarela de pago de Stripe para procesar los pagos de los pedidos realizados por parte de los clientes. Esto garantizará la seguridad de los pagos.

## **RF-14**: Gestionar y modificar pedidos
> El sistema permitirá al usuario de tipo administrador, modificar y eliminar pedidos, en caso de que sea necesario.

## **RF-15**: Gestionar incidencias en el reparto
> El sistema permitirá al usuario de tipo administrador revisar y resolver las distintas incidencias.

## **RF-16**: Acceso a BBDD
> El sistema permitirá el acceso a la base de datos de Clientes y de Pedidos para la gestión de información ubicua.