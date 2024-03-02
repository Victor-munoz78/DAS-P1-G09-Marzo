# Elección de tipo cifrado para los datos del cliente

* Status: accepted
* Date: 2024-03-02

Technical Story: RF-1.1

## Context and Problem Statement

Necesitamos una forma paa proteger los datos personales del cliente, como el identificador, nombre, apellidos, email y teléfono, ¿cuál sería el mejor cifrado para ello?

## Considered Options

* AES-256
* RSA
* No cifrar datos

## Decision Outcome

Chosen option: "AES-256", because comes out best.

### Positive Consequences

* Ofrece una seguridad robusta y confiable.

### Negative Consequences

* Su implementación puede requerir más recursos computacionales y memoria.

## Pros and Cons of the Options

### AES-256

Algoritmo de cifrado simétrico

### RSA

Algoritmo de cifrado asimétrico
