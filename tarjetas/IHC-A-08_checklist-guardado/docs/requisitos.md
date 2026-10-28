# Fase 2 · Requisitos verificables — IHC-A-08 · Dashboard UX · Checklist que se conserva y estado de guardado

**Responsable:** González Álvarez Vladimir Humberto

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Explicar el procedimiento en el paso 1 antes de iniciar. | La card «Cómo funciona» lista los 5 pasos y la duración. | Restricción de la tarjeta |
| RF-02 | Marcar la checklist con obligatorios y opcionales. | Cada fila indica Obligatorio/Opcional y responsable. | Tarea crítica |
| RF-03 | Conservar las marcas al cambiar de paso y al volver. | Ir al paso 4 y volver al 3 mantiene las 3 marcas. | Fallo de la tarjeta (Issue #8) |
| RF-04 | Mostrar el progreso de la checklist («n de 5 · n de 3 obligatorios»). | El contador cambia al marcar. | Tarea crítica |
| RNF-01 | Operable con teclado y foco visible. | Espacio marca cada casilla. | Tarea crítica |
| RNF-02 | Estados del cierre: procesando, error y éxito. | Se ven los tres estados. | Accesibilidad (WCAG 2.2) |
| **RF-07** | **Diferenciar «Guardando…», «✓ Guardado · hora» y «Sin cambios» en la cabecera y mostrar la barra de progreso general.** | Al marcar, la cabecera pasa por «Guardando…» y luego «✓ Guardado · 09:43». | Incidencia sorpresa |

## Cambio por la incidencia
«Preservar checklist, diferenciar guardado de no guardado y mostrar progreso» → se agregó **RF-07**. Flujo actualizado en `diagramas/user-flow.png` (nodos en naranja).
