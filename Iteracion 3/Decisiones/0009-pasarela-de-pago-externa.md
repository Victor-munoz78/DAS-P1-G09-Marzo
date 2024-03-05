# Pasarela de Pago Externa

* Status: accepted
* Date: 2024-02-24

Technical Story: RF-3

## Context and Problem Statement

El sistema debe conectarse con una pasarela de pago externa para procesar los pagos.

## Considered Options

* Adapter
* Facade

## Decision Outcome

Chosen option: "Adapter", because comes out best.

### Positive Consequences

* Facilita la incorporación de nuevos componentes o servicios externos en un sistema existente sin modificar su código, permitiendo la integración sin problemas.
* Permite la reutilización eficiente de componentes existentes al adaptar sus interfaces, evitando la necesidad de reescribir o refactorizar el código ya implementado.

### Negative Consequences

* La introducción de adaptadores puede aumentar la complejidad del sistema, especialmente con múltiples adaptadores interconectados, dificultando la comprensión del código.
