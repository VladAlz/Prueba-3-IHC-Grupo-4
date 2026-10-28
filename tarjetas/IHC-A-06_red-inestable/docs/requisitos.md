# Fase 2 · Requisitos verificables — IHC-A-06 · CaféU · Confirmación sin duplicados con red inestable

**Responsable:** Mora Beltrán Santiago Sebastián

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Revisar el pedido antes de confirmar. | Se ve resumen y total. | Tarea crítica |
| RF-02 | Bloquear «Confirmar» desde el primer toque hasta recibir respuesta. | Un segundo toque no envía otro pedido. | Fallo de la tarjeta (Issue #6) |
| RF-03 | Mostrar «Enviando…» mientras no hay respuesta, sin mensajes de éxito. | Con red lenta (4 s) no aparece «confirmado» antes de tiempo. | Tarea crítica |
| RF-04 | Ante un corte, informar y permitir reintentar. | Aparece el error y «Reintentar envío». | Tarea crítica |
| RNF-01 | Funcionar con red lenta (4 s) sin perder el pedido. | El carrito se conserva tras el error. | Restricción de la tarjeta |
| RNF-02 | Estados anunciados y foco en el mensaje de error. | El lector lee el error al aparecer. | Accesibilidad (WCAG 2.2) |
