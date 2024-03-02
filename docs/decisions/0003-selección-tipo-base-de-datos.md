# Selección Tipo Base de Datos

* Status: accepted
* Date: 2024-03-02

Technical Story: RF-1

## Context and Problem Statement

En la arquitectura, se tiene planteada la existencia de 2 bases de datos (clientes y pedidos) a las que el sistema podrá acceder para guardar u obtener datos. ¿Qué tipo de base de datos debería de tener la arquitectura?

## Considered Options

* SQL

## Decision Outcome

Chosen option: "SQL", because es más adecuada para el tipo de arquitectura elegida.

### Positive Consequences

* Ideal si hay múltiples clientes que necesitan recibir notificaciones sobre el seguimiento de pedidos. Proporciona desacoplamiento entre el emisor (módulo de repartos y ruta) y los receptores (clientes) permitiendo una fácil extensión.

### Negative Consequences

* Puede volverse complejo si la lógica de notificación se vuelve más complicada o si hay muchos tipos diferentes de notificaciones
