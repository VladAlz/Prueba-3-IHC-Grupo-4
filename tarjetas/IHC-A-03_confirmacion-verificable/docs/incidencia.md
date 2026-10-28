# Incidencia sorpresa — IHC-A-03 · CaféU · Confirmación verificable en un dispositivo compartido

## Estado de pedido pendiente
| Campo | Detalle |
|---|---|
| Evento imprevisto | La aplicación tarda ocho segundos tras confirmar; el usuario vuelve a pulsar el botón. |
| Cambio obligatorio | Deshabilitar repetición, mostrar pendiente y resolverlo a confirmado o no confirmado sin duplicar. |
| Evidencias pedidas | Tres estados, prueba de doble clic, registro de Issue y commit. |
| Responsable / revisor | Acaro Ibujés Pedro Sebastián / Vinces Cueva Boris Yussef |
| Issue | «IHC-A-03 · Incidencia: Estado de pedido pendiente» (hora del anuncio y SHA del commit registrados en la issue y en el PR) |

## Respuesta
| Evidencia | Dónde está |
|---|---|
| Requisito nuevo **RF-07** | Tras confirmar, bloquear la repetición y mostrar el estado Pendiente hasta resolverlo en Confirmado o No confirmado; reintentar usa el mismo código de envío y no duplica. — `docs/requisitos.md`, `docs/trazabilidad.md` |
| Flujo / wireframe actualizados | `diagramas/user-flow.png` (nodos en naranja) y `wireframes/wf-05-incidencia.png` |
| Cambio visible en el prototipo | `send()` bloquea el botón (`aria-busy`) y asigna un código de envío; durante la espera muestra el chip «Pendiente de confirmación» (`role="status"`); al responder pasa a «✓ Recibido por la cafetería» o a «No confirmado» con reintento seguro; el registro con el mismo código no se duplica. — `prototipo/v2/index.html` |
| Prueba funcional | Pulsó dos veces durante la espera; el botón estaba bloqueado, vio «Pendiente» y luego un solo pedido recibido (77 s, 0 errores). Cita: «Decía pendiente, así que esperé; salió un solo pedido.» — `pruebas/sesion.md` |
| Antes / después | `evidencias/incidencia/` |
| Evidencia específica | Prueba de doble clic con red lenta de 8 s (panel del moderador, «Red de prueba: Lenta»). |
| Commit y revisión | Rama de incidencias de Pedro, commit posterior al anuncio, PR revisado por Boris |
| Defensa | ¿Cómo evita confundir clic efectuado con pedido confirmado? — `docs/defensa.md` |

## Verificación (rúbrica de la incidencia, 0,25)
| Criterio | Cumplimiento |
|---|---|
| Funcionamiento comprobable (0,08) | Con red lenta (8 s) y doble clic, el botón queda bloqueado, se ve «Pendiente de confirmación» y al final hay un solo pedido. |
| Requisito, flujo o wireframe actualizado (0,05) | RF-07, user flow y `wf-05-incidencia.png` |
| Prueba y evidencia antes/después (0,05) | `pruebas/sesion.md` y `evidencias/incidencia/` |
| Commit posterior y revisión de compañero (0,04) | PR de incidencias revisado por Vinces Cueva Boris Yussef |
| Defensa individual (0,03) | `docs/defensa.md` |

| Antes (v2) | Después (v2 con la incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
