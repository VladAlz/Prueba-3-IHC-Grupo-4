# Incidencia sorpresa — IHC-A-08 · Dashboard UX · Checklist que se conserva y estado de guardado

## Guardado inconsistente
| Campo | Detalle |
|---|---|
| Evento imprevisto | El usuario marca tres casillas, cambia de etapa y vuelve: aparecen desmarcadas. |
| Cambio obligatorio | Conservar valores, informar su estado de guardado y diferenciar pendiente/completo. |
| Evidencias pedidas | Capturas antes/después, prueba de retorno, revisión de PR. |
| Responsable / revisor | González Álvarez Vladimir Humberto / Mora Beltrán Santiago Sebastián |
| Issue | «IHC-A-08 · Incidencia: Guardado inconsistente» (hora del anuncio y SHA del commit registrados en la issue y en el PR) |

## Respuesta
| Evidencia | Dónde está |
|---|---|
| Requisito nuevo **RF-07** | Diferenciar «Guardando…», «✓ Guardado · hora» y «Sin cambios» en la cabecera y mostrar la barra de progreso general. — `docs/requisitos.md`, `docs/trazabilidad.md` |
| Flujo / wireframe actualizados | `diagramas/user-flow.png` (nodos en naranja) y `wireframes/wf-05-incidencia.png` |
| Cambio visible en el prototipo | `markSaved()` muestra «Guardando…» y, al terminar, «✓ Guardado · hora»; la barra `#pbar` refleja el avance general. — `prototipo/v2/index.html` |
| Prueba funcional | Vio «Guardando…» y «Guardado · hora» y la barra de progreso (91 s, 0 errores). Cita: «Sé cuándo ya se guardó.» — `pruebas/sesion.md` |
| Antes / después | `evidencias/incidencia/` |

| Commit y revisión | Rama de incidencias de Vladimir, commit posterior al anuncio, PR revisado por Santiago |
| Defensa | ¿Qué evidencia muestra una mejora real frente a una mejora inferida? — `docs/defensa.md` |

## Verificación (rúbrica de la incidencia, 0,25)
| Criterio | Cumplimiento |
|---|---|
| Funcionamiento comprobable (0,08) | Al marcar, la cabecera pasa por «Guardando…» y luego «✓ Guardado · 09:43». |
| Requisito, flujo o wireframe actualizado (0,05) | RF-07, user flow y `wf-05-incidencia.png` |
| Prueba y evidencia antes/después (0,05) | `pruebas/sesion.md` y `evidencias/incidencia/` |
| Commit posterior y revisión de compañero (0,04) | PR de incidencias revisado por Mora Beltrán Santiago Sebastián |
| Defensa individual (0,03) | `docs/defensa.md` |

| Antes (v2) | Después (v2 con la incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
