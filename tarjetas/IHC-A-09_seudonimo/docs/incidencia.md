# Incidencia sorpresa — IHC-A-09 · Dashboard UX · Participantes anónimos con código seudónimo

## Dato personal inesperado
| Campo | Detalle |
|---|---|
| Evento imprevisto | La interfaz ahora solicita el nombre completo de un participante y lo incluye en resumen. |
| Cambio obligatorio | Sustituir por código anónimo y eliminar nombre del resumen sin perder métricas. |
| Evidencias pedidas | Validación, requisito de privacidad, prueba y commit. |
| Responsable / revisor | González Álvarez Vladimir Humberto / Mora Beltrán Santiago Sebastián |
| Issue | «IHC-A-09 · Incidencia: Dato personal inesperado» (hora del anuncio y SHA del commit registrados en la issue y en el PR) |

## Respuesta
| Evidencia | Dónde está |
|---|---|
| Requisito nuevo **RF-07** | Validar el formato del código seudónimo (P-07: P, guion y 2–3 dígitos) al salir del campo y al continuar, con mensaje junto al campo. — `docs/requisitos.md`, `docs/trazabilidad.md` |
| Flujo / wireframe actualizados | `diagramas/user-flow.png` (nodos en naranja) y `wireframes/wf-05-incidencia.png` |
| Cambio visible en el prototipo | `missing(1)` valida `/^P-\d{2,3}$/`; `fieldErr()` muestra el error junto al campo con `aria-invalid` y `aria-describedby`. — `prototipo/v2/index.html` |
| Prueba funcional | Escribió «p7»; el mensaje indicó el formato y corrigió a P-07 (94 s, 1 errores). Cita: «Me dijo el formato, listo.» — `pruebas/sesion.md` |
| Antes / después | `evidencias/incidencia/` |

| Commit y revisión | Rama de incidencias de Vladimir, commit posterior al anuncio, PR revisado por Santiago |
| Defensa | ¿Qué requisito protege privacidad y dónde aparece en la trazabilidad? — `docs/defensa.md` |

## Verificación (rúbrica de la incidencia, 0,25)
| Criterio | Cumplimiento |
|---|---|
| Funcionamiento comprobable (0,08) | «ana» muestra «El código debe tener el formato P-07…». |
| Requisito, flujo o wireframe actualizado (0,05) | RF-07, user flow y `wf-05-incidencia.png` |
| Prueba y evidencia antes/después (0,05) | `pruebas/sesion.md` y `evidencias/incidencia/` |
| Commit posterior y revisión de compañero (0,04) | PR de incidencias revisado por Mora Beltrán Santiago Sebastián |
| Defensa individual (0,03) | `docs/defensa.md` |

| Antes (v2) | Después (v2 con la incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
