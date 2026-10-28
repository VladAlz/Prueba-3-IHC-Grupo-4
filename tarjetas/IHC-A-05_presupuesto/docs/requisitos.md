# Fase 2 · Requisitos verificables — IHC-A-05 · CaféU · Pedido dentro de un presupuesto de USD 4,25

**Responsable:** Mora Beltrán Santiago Sebastián

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Mostrar el presupuesto ($4,25) y lo gastado al elegir. | El menú muestra «Llevas $X de $4,25». | Tarea crítica |
| RF-02 | Ajustar cantidades y quitar productos en «Mi pedido». | −, + y Quitar actualizan el total. | Tarea crítica |
| RF-03 | Avisar en el momento de la edición cuando el total supera el presupuesto, indicando cuánto. | Con 2 cafés y 1 sánduche aparece «Te pasas por $1,50». | Fallo de la tarjeta (Issue #5) |
| RF-04 | Mostrar procesando, error con reintento y confirmación con total. | Se ven los tres estados. | Tarea crítica |
| RNF-01 | El aviso de exceso usa texto e ícono, no solo color. | Legible en escala de grises. | Restricción de la tarjeta |
| RNF-02 | Operable con teclado; el aviso se anuncia (aria-live). | El lector lee «Total $5,75». | Accesibilidad (WCAG 2.2) |
| **RF-07** | **Si el precio de un producto cambia antes de confirmar, actualizar el total, explicar el cambio con un desglose (antes → ahora) y permitir modificar cantidades, cancelar o confirmar el nuevo total.** | Con el sánduche a $3,25, «Confirmar» muestra el desglose $2,75 → $3,25 y total $4,25 → $4,75, con «Modificar cantidades», «Cancelar pedido» y «Confirmar nuevo total». | Incidencia sorpresa |

## Cambio por la incidencia
«Actualizar total, explicar el cambio y permitir modificar cantidades o cancelar.» → se agregó **RF-07**. Flujo actualizado en `diagramas/user-flow.png` (nodos en naranja).
