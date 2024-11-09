# Requisitos Funcionales

## **RF-01**: Pasar de arquitectura monolítica a una de microservicios 
> El sistema deberá de pasar de una arquitectura monolítica a una de microservicios para poder tener una mayor modularidad.

## **RF-02**: Conexión cliente-servidor con HTTP/REST
> El sistema deberá permitir al cliente conectarser al servidor a través del protocolo HTTP/REST con un componente Gateaway.

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
> El sistema podrá elegir entre dos algoritmos de optimización de rutas. Se debe utilizar uno u otro según la demora del camión.

## **RF-09**: Proveer datos sobre el estado de los pedidos
> El sistema deberá mantener actualizado el estado de los pedidos para que los clientes puedan consultarlo y saber el progreso de su pedido.

## **RF-10**: Recibir la posición de los camiones
> El sistema registrará mediante señal GPS la posición de los camiones en tiempo real, almacenándola para que esta sea accesible en cualquier momento.

## **RF-11**: Mostrar estadisticas a los clientes
> El sistema deberá generar estadisticas automáticamente para los usuarios de tipo cliente acerca de los pedidos y la posición en tiempo real de los camiones.

## **RF-12**: Mostrar estadisticas a los administradores
> El sistema deberá generar estadisticas automáticamente para los usuarios de tipo administrtador acerca de los clientes, los pedidos y la posición en tiempo real de los camiones.

## **RF-13**: Reportar incidencia
> El sistema permitirá al usuario de tipo repartidor reportar incidencias en tiempo real para registrarlas en el sistema.

## **RF-14**: Gestionar pagos con una pasarela externa
> El sistema se conectará con la pasarela de pago de Stripe para procesar los pagos de los pedidos realizados por parte de los clientes. Esto garantizará la seguridad de los pagos.

## **RF-15**: Gestionar y modificar pedidos
> El sistema permitirá al usuario de tipo administrador, modificar y eliminar pedidos, en caso de que sea necesario.

## **RF-16**: Gestionar incidencias en el reparto
> El sistema permitirá al usuario de tipo administrador revisar y resolver las distintas incidencias.

## **RF-17**: Acceso a BBDD
> El sistema permitirá el acceso a la base de datos de Clientes y de Pedidos para la gestión de información ubicua.