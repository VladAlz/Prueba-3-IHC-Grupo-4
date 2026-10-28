# Incidencia sorpresa — IHC-A-01 · CaféU · Total que se actualiza en un pedido rápido

## Precio cambia al editar
| Campo | Detalle |
|---|---|
| Evento imprevisto | Tras modificar de 1 a 2 cafés, la pantalla conserva USD 4,25 aunque el total real cambia. |
| Cambio obligatorio | Implementar actualización de subtotales y total, identificar diferencia, pedir nueva revisión antes de confirmar. |
| Evidencias pedidas | Nuevo requisito R7, user flow corregido, captura del total y test de edición. |
| Responsable / revisor | Acaro Ibujés Pedro Sebastián / Vinces Cueva Boris Yussef |
| Issue | «IHC-A-01 · Incidencia: Precio cambia al editar» (hora del anuncio y SHA del commit registrados en la issue y en el PR) |

## Respuesta
| Evidencia | Dónde está |
|---|---|
| Requisito nuevo **RF-07** | Recalcular subtotales y total en cada edición, mostrar la diferencia (antes → ahora) y exigir una nueva revisión del total antes de confirmar. — `docs/requisitos.md`, `docs/trazabilidad.md` |
| Flujo / wireframe actualizados | `diagramas/user-flow.png` (nodos en naranja) y `wireframes/wf-05-incidencia.png` |
| Cambio visible en el prototipo | En `renderReview()` se guarda el total revisado (`S.revBase`); si una edición lo cambia, aparece el aviso con la diferencia, `#confirm` se deshabilita (`aria-describedby`) y solo se habilita al pulsar «Revisé el nuevo total». — `prototipo/v2/index.html` |
| Prueba funcional | Subió un café en «Revisa y confirma»; leyó «+$1,50», pulsó «Revisé el nuevo total» y confirmó $7,25 (84 s, 0 errores). Cita: «Me muestra cuánto subió antes de dejarme confirmar.» — `pruebas/sesion.md` |
| Antes / después | `evidencias/incidencia/` |

| Commit y revisión | Rama de incidencias de Pedro, commit posterior al anuncio, PR revisado por Boris |
| Defensa | ¿Qué parte de la rama de editar del user flow se modifica? — `docs/defensa.md` |

## Verificación (rúbrica de la incidencia, 0,25)
| Criterio | Cumplimiento |
|---|---|
| Funcionamiento comprobable (0,08) | Con 2 → 3 cafés en «Revisa y confirma» aparece «Antes $5,75 → ahora $7,25 (+$1,50)» y «Confirmar» queda bloqueado hasta pulsar «Revisé el nuevo total». |
| Requisito, flujo o wireframe actualizado (0,05) | RF-07, user flow y `wf-05-incidencia.png` |
| Prueba y evidencia antes/después (0,05) | `pruebas/sesion.md` y `evidencias/incidencia/` |
| Commit posterior y revisión de compañero (0,04) | PR de incidencias revisado por Vinces Cueva Boris Yussef |
| Defensa individual (0,03) | `docs/defensa.md` |

| Antes (v2) | Después (v2 con la incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
