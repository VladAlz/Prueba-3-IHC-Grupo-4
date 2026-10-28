# Fase 2 · Requisitos verificables — IHC-A-04 · CaféU · Advertencia de alérgenos antes de confirmar

**Responsable:** Mora Beltrán Santiago Sebastián

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Declarar una alergia al iniciar (sin guardarla). | El selector ofrece Ninguna/Frutos secos/Lácteos/Gluten. | Tarea crítica |
| RF-02 | Consultar ingredientes y alérgenos de cada producto. | «Info» muestra ingredientes y la advertencia si coincide. | Tarea crítica |
| RF-03 | Marcar en el menú y en el pedido los productos que contienen el alérgeno declarado. | El brownie muestra «⚠ Contiene frutos secos». | Tarea crítica |
| RF-04 | Impedir confirmar sin reconocer la advertencia. | Si no se marca «Leí la advertencia…», aparece un error y no se envía. | Fallo de la tarjeta (Issue #4) |
| RNF-01 | La advertencia usa ícono y texto, no solo color (WCAG 1.4.1). | Se entiende en la vista en escala de grises. | Restricción de la tarjeta |
| RNF-02 | Operable con teclado y foco visible. | La casilla y los botones se alcanzan con Tab. | Accesibilidad (WCAG 2.2) |
| **RF-07** | **La advertencia es accesible (role="alert", recibe el foco al entrar) y ofrece «Volver a editar sin perder el pedido», que lleva al producto marcado.** | Al abrir «Revisa y confirma» el lector lee la advertencia; el enlace lleva a «Mi pedido» con el foco en «Quitar Brownie». | Incidencia sorpresa |

## Cambio por la incidencia
«Incorporar aviso accesible y opción de volver a editar sin perder pedido» → se agregó **RF-07**. Flujo actualizado en `diagramas/user-flow.png` (nodos en naranja).
