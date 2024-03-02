# Notificaciones a Clientes

* Status: proposed
* Date: 2024-03-02

Technical Story: RF-4

## Context and Problem Statement

Se necesita que el módulo de reparto y rutas pueda notificar a los clientes el estado de su pedido mediante mensajes de texto o a sus redes sociales, ¿cuál será el mejor patrón para su implementación?

## Considered Options

* Observer
* Adapter

## Decision Outcome

Chosen option: "Observer", because comes out best.

### Positive Consequences

* Ideal si hay múltiples clientes que necesitan recibir notificaciones sobre el seguimiento de pedidos. Proporciona desacoplamiento entre el emisor (módulo de repartos y ruta) y los receptores (clientes) permitiendo una fácil extensión.

### Negative Consequences

* Puede volverse complejo si la lógica de notificación se vuelve más complicada o si hay muchos tipos diferentes de notificaciones
