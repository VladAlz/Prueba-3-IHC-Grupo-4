# Fase 2 · Requisitos verificables — IHC-A-01 · CaféU · Total que se actualiza en un pedido rápido

**Responsable:** Acaro Ibujés Pedro Sebastián

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Agregar un producto al pedido desde el menú con una sola acción y ver un aviso con el total. | Tras pulsar «Agregar», el aviso muestra el nombre y el total en menos de 1 s. | Tarea crítica |
| RF-02 | Cambiar la cantidad (1–9) de cada producto desde «Mi pedido». | Los botones − y + cambian la cantidad y no permiten 0 ni 10. | Tarea crítica |
| RF-03 | Recalcular subtotal y total al instante después de cada cambio de cantidad. | Con 2 cafés y 1 sánduche el total muestra $5,75 sin recargar. | Fallo de la tarjeta (Issue #1) |
| RF-04 | Mostrar el estado del envío: procesando, error con reintento y éxito con número de pedido. | Se ven las tres pantallas; el botón se bloquea mientras envía. | Tarea crítica |
| RNF-01 | La tarea completa cabe en 360 px y se termina en menos de 3 minutos. | Sin desplazamiento horizontal; tiempo de la prueba < 180 s. | Restricción de la tarjeta |
| RNF-02 | Operable con teclado y foco visible (WCAG 2.1.1, 2.4.7). | Toda la tarea se completa con Tab/Enter; anillo de foco de 3 px. | Accesibilidad (WCAG 2.2) |
| **RF-07** | **Recalcular subtotales y total en cada edición, mostrar la diferencia (antes → ahora) y exigir una nueva revisión del total antes de confirmar.** | Con 2 → 3 cafés en «Revisa y confirma» aparece «Antes $5,75 → ahora $7,25 (+$1,50)» y «Confirmar» queda bloqueado hasta pulsar «Revisé el nuevo total». | Incidencia sorpresa |

## Cambio por la incidencia
«Implementar actualización de subtotales y total, identificar diferencia, pedir nueva revisión antes de confirmar.» → se agregó **RF-07**. Flujo actualizado en `diagramas/user-flow.png` (nodos en naranja).
