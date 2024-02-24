# Gestión de módulos

* Status: accepted
* Date: 2024-02-24

Technical Story: RF-2

## Context and Problem Statement

El sistema requiere la integración de dos algoritmos de optimización, los cuales serán elegidos en base a la latencia experimentada por el camión. Este proceso de selección se llevará a cabo mediante la aplicación de un diseño estructurado que simplifique y favorezca la implementación de dichos algoritmos.

## Decision Drivers

* La empresa tiene diferentes módulos con comportamientos variados, algunos críticos y otros no críticos.

## Considered Options

* Patrón State
* Patrón Strategy

## Decision Outcome

Chosen option: "Patrón Strategy", because permite definir una familia de algoritmos, encapsular cada uno de ellos y hacer que sean intercambiables. En este caso, se puede utilizar para gestionar las estrategias de optimización en el módulo de Reparto y Rutas, permitiendo cambiar los algoritmos de optimización según la demora del camión.
