# Defensa — IHC-A-02 · CaféU · Editar y finalizar un pedido solo con teclado

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | Acaro Ibujés Pedro Sebastián |
| Revisor del pull request y observador de la prueba | Vinces Cueva Boris Yussef |
| Issue del hallazgo | #2 · Issue de la incidencia (cerrada por el PR de incidencias) |
| Ramas | `feature/pedro-tarjetas-01-03` · `fix/pedro-incidencias-01-03` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-03:** `askQuit()` abre el diálogo y enfoca «Sí, quitar»; `closeQuit()` cancela con Escape y devuelve el foco; `doQuit()` elimina y restaura el foco.

**3. Mejora vinculada a la Issue #2:** El botón dice «Quitar» con `aria-label="Quitar X del pedido"` y abre un diálogo `role="alertdialog"` con «Sí, quitar / Cancelar»; Escape cancela. Medición: 171 s / 3 errores → 104 s / 1 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó Vinces Cueva Boris Yussef, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar en `doQuit()` el destino del foco (por ejemplo, al total) o el texto del diálogo de confirmación.

## Pregunta individual
**Demuestre edición, eliminación y confirmación sin usar el ratón.**

Demostración: Tab → «Saltar al contenido» → Enter en «Ver menú» → Enter en «Agregar Café americano» y «Agregar Sánduche» → Tab a «Mi pedido» → Enter en «Aumentar cantidad de Café» → Enter en «Quitar Sánduche» → Enter en «Sí, quitar» (o Escape para cancelar) → el foco queda en el siguiente «Quitar» → Tab a «Revisar pedido» → Enter en «Confirmar».

## Incidencia
«Anunciar producto eliminado, devolver foco a control pertinente y permitir Deshacer simulado.» — `doQuit()` anuncia el producto eliminado con `live()`, mueve el foco al «Quitar» del siguiente producto (o al título) y el aviso ofrece «Deshacer», que restaura el producto y devuelve el foco a su botón; todos los controles tienen nombre accesible. Ver `docs/incidencia.md`.
