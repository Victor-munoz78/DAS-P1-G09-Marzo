# Selección Tipo Base de Datos

* Status: accepted
* Date: 2024-02-08

Technical Story: RF-1

## Context and Problem Statement

En la arquitectura, se tiene planteada la existencia de 2 bases de datos (clientes y pedidos) a las que el sistema podrá acceder para guardar u obtener datos. ¿Qué tipo de base de datos debería de tener la arquitectura?

## Considered Options

* SQL

## Decision Outcome

Chosen option: "SQL", because es más adecuada para el tipo de arquitectura elegida.

### Positive Consequences

* Organización estructurada de datos y seguridad.
* Facilidad de consulta y escalabilidad.

### Negative Consequences

* Posible impacto en el rendimiento del sistema.
* Rigidez en el esquema de datos.
