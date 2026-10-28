# Fase 2 · Requisitos verificables — IHC-A-12 · Dashboard UX · Retomar una prueba y cerrar sin éxito falso

**Responsable:** Vinces Cueva Boris Yussef

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Guardar el avance y recuperarlo al reabrir. | Tras interrumpir y reabrir, los datos siguen. | Tarea crítica |
| RF-02 | Indicar qué pasos se recuperaron y permitir continuar o empezar de nuevo. | Aviso con los pasos y dos acciones. | Tarea crítica |
| RF-03 | Impedir finalizar si falta un obligatorio de la checklist. | Con 2 de 3 obligatorios aparece error. | Fallo de la tarjeta (Issue #12) |
| RF-04 | Mostrar el cierre con código y resumen. | Aparece S-2026-0XX. | Tarea crítica |
| RNF-01 | No perder pasos finalizados (persistencia local). | Recargar no borra datos. | Restricción de la tarjeta |
| RNF-02 | Operable con teclado; errores enfocados. | El error recibe el foco. | Accesibilidad (WCAG 2.2) |
| **RF-07** | **Revisión previa con ✓/✕ por cada obligatorio, tarea, código y registros; «Finalizar» solo habilitado si todo está ✓ y el éxito incluye un resumen comprobable.** | Con un obligatorio pendiente, la revisión muestra ✕ y «Finalizar» queda deshabilitado. | Incidencia sorpresa |

## Cambio por la incidencia
«Añadir revisión previa y resumen comprobable; evitar éxito falso» → se agregó **RF-07**. Flujo actualizado en `diagramas/user-flow.png` (nodos en naranja).
