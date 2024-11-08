# Requisitos Funcionales

## **RF-01**: Pasar de arquitectura monolítica a una de microservicios 
> La aplicación deberá de pasar de una arquitectura monolítica a una de microservicios para poder tener una mayor modularidad.

## **RF-02**: Acceso a datos del Clientecce
> La aplicación permitirá al usuario de tipo cliente acceder a su información personal para poder añadir, modificar o eliminar esa información.

## **RF-03**: Gestionar y modificar pedidos
> La aplicación permitirá al usuario de tipo administrador modificar y eliminar pedidos, en caso de que sea necesario.

## **RF-04**: Gestionar incidencias en el reparto
> La aplicación permitirá al usuario de tipo administrador revisar y resolver las distintas incidencias.

## **RF-06**: Realizar pedidos
> La aplicación permitirá al usuario de tipo cliente realizar pedidos de los productos disponibles.

## **RF-07**: Reintentar pedido
> La aplicación otorgará al usuario de tipo cliente tres intentos a la hora de realizar un pedido para evitar errores.

## **RF-08**: Procesar pedidos 
> Cada pedido deberá pasa por tres fases secuenciales (preprocesado, autorización, y aceptación) y no puede avanzar a la siguiente fase sin haber completado la anterior. De esta forma se asegura la validez de los pedidos.

## **RF-09**: Gestión de flotas
> La aplicación permitirá al usuario de tipo Administrador añadir, modificar o eliminar los camiones de las flotas.

## **RF-10**: Selección de algoritmo de optimización
> El sistema podrá legir entre dos algoritmos de optimización de rutas. Se debe utilizar uno u otro según la demora del camión.

## **RF-11**: Proveer datos sobre el estado de los pedidos
> La aplicación deberá mantener actualizado el estado de los pedidos para que los clientes puedan consultarlo y saber el progreso de su pedido.

## **RF-12**: Registrar y proporcionar la posición de los camiones
> La aplicación registrará mediante señal GPS la posición de los camiones en tiempo real, almacenándola para que esta sea accesible en cualquier momento.

## **RF-13**: Reportar incidencia
> La aplicación permitirá al usuario de tipo Repartidor reportar incidencias para registrarlas en el sistema.

## **RF-14**: Gestionar pagos con una pasarela externa
> La aplicación se conectará con la pasarela de pago de Stripe para procesar los pagos de los pedidos realizados por parte de los clientes. Esto garantizará la seguridad de los pagos.