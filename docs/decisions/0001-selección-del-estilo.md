# Selección del estilo

* Status: accepted
* Date: 2024-02-06

Technical Story: RF-1, RF-2 y RF-4

## Context and Problem Statement

Se requiere un sistema con arquitectura orientada a microservicios, que sea flexible, modular y fácilmente expandible. ¿Qué tipo de arquitectura sería la más adecuada?

## Considered Options

* Cliente Servidor
* Modelo Vista-Controlador (MCV)
* Orientado a servicios (SOA)

## Decision Outcome

Chosen option: "Cliente Servidor", because Hemos elegido el estilo Cliente-Servidor porque se ajusta bien a los requisitos proporcionados, especialmente la necesidad de comunicación entre dispositivos cliente y un servidor central. Además, este estilo permite una clara separación de responsabilidades y la distribución de la carga entre el cliente y el servidor, lo que facilita la escalabilidad y el mantenimiento del sistema.

### Positive Consequences

* Separación clara de responsabilidades entre el cliente y el servidor.
* Facilita la escalabilidad y el mantenimiento del sistema.
* Permite la distribución de carga entre múltiples servidores.

### Negative Consequences

* Puede resultar en una mayor complejidad debido a la gestión de la comunicación entre el cliente y el servidor.

* La dependencia del servidor puede provocar problemas de escalabilidad si no se diseña adecuadamente.




## Pros and Cons of the Options

### Cliente Servidor

En este estilo, el sistema se divide en dos partes principales: el cliente, que solicita servicios, y el servidor, que los proporciona. La comunicación entre el cliente y el servidor se realiza a través de solicitudes y respuestas.

* Good, because Este estilo es adecuado cuando se necesita una separación clara entre la lógica del cliente y la del servidor, lo que facilita la escalabilidad y el mantenimiento del sistema. Además, permite la distribución de carga entre múltiples servidores y el soporte de diferentes tipos de clientes.
* Bad, because Puede resultar en una mayor complejidad debido a la necesidad de gestionar la comunicación entre el cliente y el servidor. Además, la dependencia del servidor puede provocar problemas de escalabilidad si no se diseña adecuadamente.

### Modelo Vista-Controlador

Este estilo separa la aplicación en tres componentes principales: Modelo (representa los datos y la lógica de negocio), Vista (representa la interfaz de usuario) y Controlador (maneja las interacciones del usuario y actualiza el modelo y la vista según sea necesario).

* Good, because Proporciona una separación clara de responsabilidades, lo que facilita la reutilización del código y el mantenimiento del sistema. Además, permite una mayor modularidad y flexibilidad en el desarrollo de la aplicación.
* Bad, because Puede resultar en una mayor complejidad debido a la necesidad de coordinar la comunicación entre los componentes. Además, puede ser excesivo para aplicaciones más pequeñas o simples.

### Orientado a servicios

En este estilo, el sistema se organiza en torno a servicios independientes y autónomos que se comunican entre sí a través de interfaces estandarizadas. Estos servicios pueden ser reutilizados y combinados para construir aplicaciones más grandes y complejas.

* Good, because Proporciona una alta interoperabilidad y reutilización de servicios, lo que facilita la integración de sistemas heterogéneos y la adaptabilidad a cambios en los requisitos del negocio. Además, permite una mayor modularidad y escalabilidad.
* Bad, because Puede resultar en una mayor complejidad debido a la necesidad de gestionar la comunicación entre los diferentes servicios. Además, puede requerir una cuidadosa planificación y diseño para garantizar la cohesión y el rendimiento del sistema.
