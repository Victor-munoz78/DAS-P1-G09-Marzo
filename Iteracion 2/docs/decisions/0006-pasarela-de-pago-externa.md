# Pasarela de pago externa

* Status: accepted
* Date: 2024-02-13

Technical Story: RF-3

## Context and Problem Statement

Se requiere que el sistema se conecte con una pasarela de pago externa, ¿cuál es el mejor patrón para ello?

## Considered Options

* Patrón Adapter
* Patrón Facade

## Decision Outcome

Chosen option: "Patrón Adapter", because su objetivo es hacer que dos interfaces sean compatibles, lo cual facilitaría que la interfaz de la pasarela de pago funcionase correctamente en nuestro sistema.

## Pros and Cons of the Options

### Patrón Adapter

Permite la colaboración entre interfaces incompatibles.

* Good, because Se pueden añadir nuevos adaptadores sin descomponer las interfaces afectadas.
* Good, because Su objetivo es compatibilizar interfaces que son incompatibles.
* Bad, because La complejidad del código aumenta al introducir nuevas interfaces.

### Patrón Facade

Proporciona una interfaz simplificada a una biblioteca o framework.

* Good, because Define interfaces para objetos existentes.
* Bad, because Su objetivo es definir interfaces nuevas para objetos existentes, no hacer que dos interfaces sean compatibles.
