# Módulo de Reputación de Vendedores

Trabajo Práctico Integrador – Organización Empresarial
Tecnicatura Universitaria en Programación – Universidad Tecnológica Nacional

## Integrantes

Tiziana Abrigo

Docente titular: Prof. Gabriela Martínez

## Descripción del sistema

Módulo de software para un marketplace (caso de estudio: Mercado Libre) que recopila las calificaciones que dejan los compradores (cumplimiento del plazo de entrega, coincidencia del producto con lo publicado y calidad de la atención) y las traduce en un puntaje de reputación visible para cada vendedor. Ese puntaje impacta en el posicionamiento dentro del marketplace y en las restricciones de pago, con el fin de aumentar la confianza de los compradores.

**Objetivo general:** desarrollar e implementar, en 18 semanas, un módulo de reputación de vendedores integrado de forma simulada al posicionamiento del marketplace y a las restricciones de pago.

## Proceso de negocio (BPMN)

El proceso modelado es el de una calificación, desde que el comprador la envía hasta que se actualiza el puntaje del vendedor.

- **Pools:** Comprador (actor externo) y Plataforma (organización).
- **Lanes de la Plataforma:** Sistema (comportamiento automatizado) y Analista (rol interno de moderación).
- **Flujo estándar:** el comprador califica, el sistema valida la compra, detecta si la calificación es sospechosa, calcula y actualiza el puntaje.
- **Excepciones (compuertas):** compra no válida (se rechaza la calificación) y calificación sospechosa (la revisa un analista, que puede descartarla).


## Historias de usuario

1. Como comprador, quiero calificar al vendedor según plazo, producto y atención, para que mi experiencia ayude a otros compradores a decidir.
2. Como vendedor, quiero ver mi puntaje de reputación y su nivel, para saber cómo me perciben y mejorar mi servicio.
3. Como analista de moderación, quiero revisar las calificaciones marcadas como sospechosas, para evitar que reseñas falsas distorsionen la reputación.

## Indicadores de control

- Tiempo de respuesta: menos de 2 segundos en el 95 % de las consultas.
- Escalabilidad: 1.000.000 de calificaciones sin degradar el tiempo más de un 10 %.
- Cobertura de pruebas: al menos 80 %.
- Errores críticos abiertos al desplegar: 0.

## Declaración de uso de IA

Usé Claude (Anthropic) como asistente durante el trabajo, con dos usos principales.

**1. Diseños y borradores**
Le pedí que me generara un disñeo del organigrama, el diccionario de datos, el diagrama BPMN. Le di como base mi TP2 (FODA, objetivos y Gantt) para que todo fuera coherente con mi proyecto del módulo de reputación de Mercado Libre.

**2. Ayuda con GitHub**
Me explicó cómo crear el repositorio, las ramas, los commits, el Pull Request y el tablero en GitHub Projects, y me fue guiando mientras lo hacía.

**correcciones**

le mande explique como queria que se vieran los diseños y fui modificandolo.
