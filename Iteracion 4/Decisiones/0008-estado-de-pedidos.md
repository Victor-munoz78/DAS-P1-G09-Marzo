# Estado de Pedidos

* Status: accepted
* Date: 2024-03-02

Technical Story: RF-2.4

## Context and Problem Statement

El sistema debe ser capaz de actualizar y mostrar el estado de los pedidos en cualquier momento.

## Considered Options

* Patrón Observer
* Patrón Strategy

## Decision Outcome

Chosen option: "Patrón Observer", because comes out best.

### Positive Consequences

* Permite actualizar los módulos de estadísticas cuando ocurre un evento en los pedidos o repartos.

### Negative Consequences

* Si hay muchos usuarios interesados en el estado de los pedidos, puede resultar en una sobrecarga de notificaciones.
