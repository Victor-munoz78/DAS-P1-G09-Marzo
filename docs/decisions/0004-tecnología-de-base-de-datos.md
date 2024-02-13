# Tecnología de Base de Datos

* Status: accepted
* Date: 2024-02-13

Technical Story: RF-1

## Context and Problem Statement

Para acceder y hacer peticiones a una Base de Datos es necesario definir el tipo de tecnología que implementa. ¿Cuál se debe usar?

## Considered Options

* SQL
* NoSQL

## Decision Outcome

Chosen option: "SQL", because es más adecuada para el tipo de arquitectura elegida.

### Positive Consequences

* Atomicidad
* Portabilidad

### Negative Consequences

* Posibles cambios en la estructura de la BD

