# Incidencia sorpresa — IHC-A-02 · CaféU · Editar y finalizar un pedido solo con teclado

## Quitar con teclado
| Campo | Detalle |
|---|---|
| Evento imprevisto | La persona pulsa Quitar con teclado y el foco desaparece; no sabe qué se eliminó. |
| Cambio obligatorio | Anunciar producto eliminado, devolver foco a control pertinente y permitir Deshacer simulado. |
| Evidencias pedidas | Secuencia Tab/Enter, prueba sin ratón, commit y wireframe ajustado. |
| Responsable / revisor | Acaro Ibujés Pedro Sebastián / Vinces Cueva Boris Yussef |
| Issue | «IHC-A-02 · Incidencia: Quitar con teclado» (hora del anuncio y SHA del commit registrados en la issue y en el PR) |

## Respuesta
| Evidencia | Dónde está |
|---|---|
| Requisito nuevo **RF-07** | Al quitar con teclado, anunciar qué producto se eliminó, devolver el foco al control pertinente (siguiente «Quitar» o título) y ofrecer «Deshacer». — `docs/requisitos.md`, `docs/trazabilidad.md` |
| Flujo / wireframe actualizados | `diagramas/user-flow.png` (nodos en naranja) y `wireframes/wf-05-incidencia.png` |
| Cambio visible en el prototipo | `doQuit()` anuncia el producto eliminado con `live()`, mueve el foco al «Quitar» del siguiente producto (o al título) y el aviso ofrece «Deshacer», que restaura el producto y devuelve el foco a su botón; todos los controles tienen nombre accesible. — `prototipo/v2/index.html` |
| Prueba funcional | Tras quitar, el foco quedó en el siguiente producto; finalizó sin volver a tabular (81 s, 0 errores). Cita: «No tuve que empezar desde arriba.» — `pruebas/sesion.md` |
| Antes / después | `evidencias/incidencia/` |
| Evidencia específica | Secuencia de teclado: Tab → «Saltar al contenido» → Enter en «Ver menú» → Enter en «Agregar Café americano» y «Agregar Sánduche» → Tab a «Mi pedido» → Enter en «Aumentar cantidad de Café» → Enter en «Quitar Sánduche» → Enter en «Sí, quitar» (o Escape para cancelar) → el foco queda en el siguiente «Quitar» → Tab a «Revisar pedido» → Enter en «Confirmar». |
| Commit y revisión | Rama de incidencias de Pedro, commit posterior al anuncio, PR revisado por Boris |
| Defensa | Demuestre edición, eliminación y confirmación sin usar el ratón. — `docs/defensa.md` |

## Verificación (rúbrica de la incidencia, 0,25)
| Criterio | Cumplimiento |
|---|---|
| Funcionamiento comprobable (0,08) | Enter en «Quitar Café» anuncia «Café americano quitado. Total $2,75», el foco queda en el siguiente «Quitar» y «Deshacer» lo restaura. |
| Requisito, flujo o wireframe actualizado (0,05) | RF-07, user flow y `wf-05-incidencia.png` |
| Prueba y evidencia antes/después (0,05) | `pruebas/sesion.md` y `evidencias/incidencia/` |
| Commit posterior y revisión de compañero (0,04) | PR de incidencias revisado por Vinces Cueva Boris Yussef |
| Defensa individual (0,03) | `docs/defensa.md` |

| Antes (v2) | Después (v2 con la incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
