# Fase 2 · Requisitos verificables — IHC-A-02 · CaféU · Editar y finalizar un pedido solo con teclado

**Responsable:** Acaro Ibujés Pedro Sebastián

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Agregar productos y navegar el menú solo con Tab y Enter. | La persona agrega café y sánduche sin ratón. | Tarea crítica |
| RF-02 | Cambiar cantidades con botones − y + operables con Enter. | Cada botón responde a Enter y anuncia la nueva cantidad. | Tarea crítica |
| RF-03 | Quitar un producto con un botón que diga qué quita y pida confirmación. | El lector anuncia «Quitar Sánduche de queso del pedido»; aparece «¿Quitar…?». | Fallo de la tarjeta (Issue #2) |
| RF-04 | Escape cancela el diálogo o vuelve a la pantalla anterior. | En el diálogo de quitar, Escape cancela y devuelve el foco a «Quitar». | Tarea crítica |
| RNF-01 | Foco visible de 3 px y orden lógico (WCAG 2.4.3, 2.4.7). | El foco nunca desaparece ni salta al inicio sin motivo. | Restricción de la tarjeta |
| RNF-02 | Estados anunciados: agregado, quitado, enviando, confirmado (WCAG 4.1.3). | Cada cambio se lee en la región aria-live. | Accesibilidad (WCAG 2.2) |
| **RF-07** | **Al quitar con teclado, anunciar qué producto se eliminó, devolver el foco al control pertinente (siguiente «Quitar» o título) y ofrecer «Deshacer».** | Enter en «Quitar Café» anuncia «Café americano quitado. Total $2,75», el foco queda en el siguiente «Quitar» y «Deshacer» lo restaura. | Incidencia sorpresa |

## Cambio por la incidencia
«Anunciar producto eliminado, devolver foco a control pertinente y permitir Deshacer simulado.» → se agregó **RF-07**. Flujo actualizado en `diagramas/user-flow.png` (nodos en naranja).
