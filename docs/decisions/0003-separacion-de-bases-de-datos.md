# Separacion de bases de datos

* Status: accepted
* Date: 2024-02-13

Technical Story: RF-1

## Context and Problem Statement

El sistema debe tener los datos separados en dos bases de datos diferentes, una de "Clientes" y otra de "Pedidos". ¿Qué modelo usamos?

## Considered Options

* Base de datos por servicio
* Diseñar un modelo propio

## Decision Outcome

Chosen option: "Patrón Base de datos por servicio", because se debe mantener una separación de las bases de datos.

### Positive Consequences

* Descentraliza las bases de datos.

### Negative Consequences

* Se deben tener en cuenta los errores
