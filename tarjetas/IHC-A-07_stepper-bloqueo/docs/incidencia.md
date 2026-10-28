# Incidencia sorpresa — IHC-A-07 · Dashboard UX · Stepper que no permite saltar etapas

## Paso de checklist obligatorio
| Campo | Detalle |
|---|---|
| Evento imprevisto | El docente añade una verificación obligatoria antes de entrar a Ejecución. |
| Cambio obligatorio | Actualizar Stepper, regla de avance, retroalimentación contextual y navegación de retorno. |
| Evidencias pedidas | Nuevo requisito y trazabilidad, test funcional, commit. |
| Responsable / revisor | González Álvarez Vladimir Humberto / Mora Beltrán Santiago Sebastián |
| Issue | «IHC-A-07 · Incidencia: Paso de checklist obligatorio» (hora del anuncio y SHA del commit registrados en la issue y en el PR) |

## Respuesta
| Evidencia | Dónde está |
|---|---|
| Requisito nuevo **RF-07** | Agregar la verificación obligatoria del docente antes de «Ejecución»: el Stepper la indica, la regla de avance la exige, el mensaje explica qué falta y «Anterior» conserva las marcas. — `docs/requisitos.md`, `docs/trazabilidad.md` |
| Flujo / wireframe actualizados | `diagramas/user-flow.png` (nodos en naranja) y `wireframes/wf-05-incidencia.png` |
| Cambio visible en el prototipo | `CHK` incluye «Verificación del docente antes de la ejecución» (obligatoria); el paso 4 se llama «Ejecución (registro)» y muestra «🔒 requiere verificación» mientras está bloqueado; `explain()` lista lo que falta con foco y las marcas se conservan al volver. — `prototipo/v2/index.html` |
| Prueba funcional | Al pulsar Continuar leyó que faltaba la verificación del docente, la marcó y entró a Ejecución (109 s, 0 errores). Cita: «El paso dice que requiere verificación y me explica cuál.» — `pruebas/sesion.md` |
| Antes / después | `evidencias/incidencia/` |

| Commit y revisión | Rama de incidencias de Vladimir, commit posterior al anuncio, PR revisado por Santiago |
| Defensa | ¿Cómo aplica la visibilidad del estado del sistema de Nielsen? — `docs/defensa.md` |

## Verificación (rúbrica de la incidencia, 0,25)
| Criterio | Cumplimiento |
|---|---|
| Funcionamiento comprobable (0,08) | Sin «Verificación del docente», el paso «Ejecución» muestra «🔒 requiere verificación» y «Continuar» explica qué falta. |
| Requisito, flujo o wireframe actualizado (0,05) | RF-07, user flow y `wf-05-incidencia.png` |
| Prueba y evidencia antes/después (0,05) | `pruebas/sesion.md` y `evidencias/incidencia/` |
| Commit posterior y revisión de compañero (0,04) | PR de incidencias revisado por Mora Beltrán Santiago Sebastián |
| Defensa individual (0,03) | `docs/defensa.md` |

| Antes (v2) | Después (v2 con la incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
