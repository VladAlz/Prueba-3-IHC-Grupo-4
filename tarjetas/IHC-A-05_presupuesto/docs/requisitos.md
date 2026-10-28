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
