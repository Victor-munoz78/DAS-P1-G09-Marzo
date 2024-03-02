# Conexión al servidor

* Status: accepted
* Date: 2024-03-02

Technical Story: RF-1

## Context and Problem Statement

Para facilitar la interacción entre los usuarios y la aplicación de la empresa, es necesario establecer un protocolo que permita la conexión entre el cliente y la capa de lógica de negocio en el servidor. ¿Qué opciones podrían ser consideradas para abordar esta necesidad?

## Considered Options

* API Gateway HTTP/REST

## Decision Outcome

Chosen option: "API Gateway HTTP/REST", because comes out best.

### Positive Consequences

* Abstracción de complejidad.
* Gestión de tráfico eficiente.

### Negative Consequences

* Configuración compleja y aumento de la latencia potencial.
