# Requisitos Funcionales
Debemos de tener en cuenta que no tenemos que considerar aquellos requisitos que se consideran de bajo nivel

## **RF-01**: Acceso a datos del Cliente
> La aplicación permitirá al usuario de tipo cliente acceder a su información personal para poder añadir, modificar o eliminar esa información.

## **RF-02**: Gestionar y modificar pedidos
> La aplicación permitirá al usuario de tipo administrador modificar y eliminar pedidos, en caso de que sea necesario.

## **RF-03**: Gestionar incidencias en el reparto
> La aplicación permitirá al usuario de tipo administrador revisar y resolver las distintas incidencias.

## **RF-04**: Realizar pedidos
> La aplicación permitirá al usuario de tipo cliente realizar pedidos de los productos disponibles.     

## **RF-05**: Reintentar pedido
> La aplicación otorgará al usuario de tipo cliente tres intentos a la hora de realizar un pedido para evitar errores.

## **RF-06**: Procesar pedidos 
> Cada pedido deberá pasa por tres fases secuenciales (preprocesado, autorización, y aceptación) y no puede avanzar a la siguiente fase sin haber completado la anterior. De esta forma se asegura la validez de los pedidos.

## **RF-07**: Gestión de flotas
> La aplicación permitirá al usuario de tipo Administrador añadir, modificar o eliminar los camiones de las flotas.

## **RF-08**: Utilizar algoritmos de optimización
> El sistema contará con dos algoritmos de optimización para calcular las rutas de los camiones. Se debe utilizar uno u otro según la demora del camión.

## **RF-09**: Proveer datos sobre el estado de los pedidos
> La aplicación deberá mantener actualizado el estado de los pedidos para que los clientes puedan consultarlo y saber el progreso de su pedido.

## **RF-10**: Registrar y proporcionar la posición de los camiones
> La aplicación registrará mediante señal GPS la posición de los camiones en tiempo real, almacenándola para que esta sea accesible en cualquier momento.

## **RF-11**: Reportar incidencia
> La aplicación permitirá al usuario de tipo Repartidor reportar incidencias para registrarlas en el sistema.

## **RF-12**: Gestionar pagos con una pasarela externa
> La aplicación se conectará con la pasarela de pago de Stripe para procesar los pagos de los pedidos realizados por parte de los clientes. Esto garantizará la seguridad de los pagos.