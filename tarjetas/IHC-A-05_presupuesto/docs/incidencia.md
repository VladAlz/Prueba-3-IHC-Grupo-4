# Incidencia sorpresa — IHC-A-05 · CaféU · Pedido dentro de un presupuesto de USD 4,25

## Presupuesto agotado
| Campo | Detalle |
|---|---|
| Evento imprevisto | El precio del producto se incrementa USD 0,50 antes de confirmar. |
| Cambio obligatorio | Actualizar total, explicar el cambio y permitir modificar cantidades o cancelar. |
| Evidencias pedidas | Requisito R7, pantalla de desglose, prueba y commit. |
| Responsable / revisor | Mora Beltrán Santiago Sebastián / Acaro Ibujés Pedro Sebastián |
| Issue | «IHC-A-05 · Incidencia: Presupuesto agotado» (hora del anuncio y SHA del commit registrados en la issue y en el PR) |

## Respuesta
| Evidencia | Dónde está |
|---|---|
| Requisito nuevo **RF-07** | Si el precio de un producto cambia antes de confirmar, actualizar el total, explicar el cambio con un desglose (antes → ahora) y permitir modificar cantidades, cancelar o confirmar el nuevo total. — `docs/requisitos.md`, `docs/trazabilidad.md` |
| Flujo / wireframe actualizados | `diagramas/user-flow.png` (nodos en naranja) y `wireframes/wf-05-incidencia.png` |
| Cambio visible en el prototipo | Al confirmar, si la cafetería actualizó un precio, se aplica el nuevo precio y se abre un diálogo con el desglose (producto y total antes → ahora) y las acciones «Modificar cantidades» (conserva el carrito), «Cancelar pedido» y «Confirmar nuevo total». — `prototipo/v2/index.html` |
| Prueba funcional | Leyó que el sánduche subió $0,50 y eligió «Modificar cantidades»; ajustó y confirmó dentro de lo que quería pagar (91 s, 0 errores). Cita: «Me explicó por qué subió el total.» — `pruebas/sesion.md` |
| Antes / después | `evidencias/incidencia/` |
| Evidencia específica | Desglose: activar en el panel «Subir +$0,50 el precio del Sánduche» y confirmar. |
| Commit y revisión | Rama de incidencias de Santiago, commit posterior al anuncio, PR revisado por Pedro |
| Defensa | ¿Qué touchpoint pasa a ser momento de verdad y por qué? — `docs/defensa.md` |

## Verificación (rúbrica de la incidencia, 0,25)
| Criterio | Cumplimiento |
|---|---|
| Funcionamiento comprobable (0,08) | Con el sánduche a $3,25, «Confirmar» muestra el desglose $2,75 → $3,25 y total $4,25 → $4,75, con «Modificar cantidades», «Cancelar pedido» y «Confirmar nuevo total». |
| Requisito, flujo o wireframe actualizado (0,05) | RF-07, user flow y `wf-05-incidencia.png` |
| Prueba y evidencia antes/después (0,05) | `pruebas/sesion.md` y `evidencias/incidencia/` |
| Commit posterior y revisión de compañero (0,04) | PR de incidencias revisado por Acaro Ibujés Pedro Sebastián |
| Defensa individual (0,03) | `docs/defensa.md` |

| Antes (v2) | Después (v2 con la incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
