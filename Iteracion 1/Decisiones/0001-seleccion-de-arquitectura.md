# Seleccion de arquitectura

* Status: accepted
* Date: 2024-02-08

Technical Story: RF-1

## Context and Problem Statement

Se requiere un sistema con arquitectura basada en microservicios, que sea flexible, modular y fácilmente expandible. ¿Qué tipo de arquitectura sería la más adecuada?

## Decision Drivers

* La lógica de negocio del sistema esta modularizada
* Posibilidad de integración de un módulo Clientes que gestione el acceso a los datos personales de los usuarios
* Posibilidad de integración de un módulo Pedidos que gestione las peticiones de pedidos
* Posibilidad de integración de un módulo Reparto que gestione el número de camiones en cada zona
* Posibilidad de integración de un módulo Rutas que determine y comuinique la mejor ruta a seguir a cada uno de los camiones de la empresa
* Posibilidad de un módulo Estadísticas que envíe información sobre el estado de los pedidos a los clientes
* Posibilidad de integración de un módulo Incidencias que transmita incidencias sobre el reparto a los gestores de rutas que lo necesiten
* Posibilidad de integración de un módulo Pagos externo, que funciona como pasarela de pago
* Posibilidad de integración de notificación a los clientes del estado de su pedido vía mensajes u otros canales de comunicación

## Considered Options

* Arquitectura Cliente-servidor (Client-Server)
* Arquitectura orientada a servicios (SOA)
* Arquitectura dirigida por eventos (Event-driven)
* Arquitectuta Modelo-Vista-Controlador (MCV)

## Decision Outcome

Chosen option: "Arquitectura Cliente-servidor", because su simplicidad de implementación, la centralización del control en el servidor y su compatibilidad con protocolos estándar cono HTTP

### Positive Consequences

* La estructura clara de cliente-servidor puede facilitar el desarrollo y la depuración del sistema
* Al centralizar la lógica de negocio y los datos en el servidor, se puede tener un mayor control sobre el sistema
* El uso de protocolos estándar como HTTP puede facilitar la integración con otras tecnologías y sistemas
* Permite la distribución de tareas entre los servidores.
* La parte cliente está separada de la parte servidor, por lo tanto es compatible con diferentes plataformas y sistemas operativos.

### Negative Consequences

* Puede tener limitaciones en términos de escalabilidad, ya que el servidor puede convertirse en un cuello de botella si recibe un alto volumen de solicitudes
* Puede haber un acoplamiento más fuerte entre el cliente y el servidor, lo que puede dificultar la modificación y la expansión del sistema
* Al centralizar la lógica de negocio y los datos en el servidor, puede haber una mayor carga de trabajo y complejidad en la gestión del servidor
