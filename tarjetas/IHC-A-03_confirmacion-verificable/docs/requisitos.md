# Fase 2 · Requisitos verificables — IHC-A-03 · CaféU · Confirmación verificable en un dispositivo compartido

**Responsable:** Acaro Ibujés Pedro Sebastián

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Agregar productos y revisar el pedido antes de confirmar. | El resumen muestra cantidades y total antes del envío. | Tarea crítica |
| RF-02 | Mostrar «Enviando…» con el botón bloqueado mientras no hay respuesta. | No aparece ningún mensaje de éxito durante el envío. | Tarea crítica |
| RF-03 | Mostrar en la confirmación un identificador del pedido, el resumen y el total. | La pantalla final incluye número, productos y total. | Fallo de la tarjeta (Issue #3) |
| RF-04 | Permitir salir y borrar el pedido de la pantalla al terminar. | «Salir y borrar este pedido» vuelve al inicio sin rastro del pedido. | Tarea crítica |
| RNF-01 | No solicitar ni mostrar datos personales (teléfono, cédula, nombre). | Ningún campo pide datos personales; el identificador no los contiene. | Restricción de la tarjeta |
| RNF-02 | Operable con teclado, foco visible y estados anunciados. | La confirmación se anuncia con su número. | Accesibilidad (WCAG 2.2) |
