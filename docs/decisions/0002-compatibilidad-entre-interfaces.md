# Compatibilidad entre interfaces

* Status: accepted
* Date: 2024-02-24

Technical Story: RF-1, RF-2

## Context and Problem Statement

Necesitamos un patrón que adapte los distintos módulos, ¿cuál sería el más indicado?

## Decision Drivers

* Dado que la empresa está migrando de una arquitectura monolítica a una basada en microservicios, es probable que se encuentren diferentes interfaces y protocolos de comunicación entre los módulos.

## Considered Options

* Patrón Adapter
* Patrón Facade

## Decision Outcome

Chosen option: "Patrón Adapter", because se puede usar para adaptar estas interfaces de manera que los microservicios puedan interactuar sin problemas.

### Positive Consequences

* Es posible incorporar nuevos adaptadores sin afectar negativamente a las interfaces existentes.
* Al tener como meta hacer compatibles interfaces que de otro modo no lo serían.

### Negative Consequences

* Considerando que la complejidad del código tiende a aumentar al introducir nuevas interfaces.

## Pros and Cons of the Options

### Patrón Adapter

Facilita la colaboración entre interfaces que inicialmente no son compatibles.
