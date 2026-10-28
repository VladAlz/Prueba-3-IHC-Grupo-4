# Defensa — IHC-A-01 · CaféU · Total que se actualiza en un pedido rápido

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | Acaro Ibujés Pedro Sebastián |
| Revisor del pull request y observador de la prueba | Vinces Cueva Boris Yussef |
| Issue del hallazgo | #1 · Issue de la incidencia (cerrada por el PR de incidencias) |
| Ramas | `feature/pedro-tarjetas-01-03` · `fix/pedro-incidencias-01-03` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-03:** `total()` suma precio × cantidad; `changeQty()` llama a `renderCart()`, que vuelve a pintar subtotal, total y el texto del botón.

**3. Mejora vinculada a la Issue #1:** Subtotal y total se recalculan en `renderCart()` con `total()` en cada cambio; el botón muestra el total vigente. Medición: 142 s / 2 errores → 88 s / 0 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó Vinces Cueva Boris Yussef, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar en `changeQty()` el mensaje de `live()` para que diga «Nuevo total: $X» o mover el foco al total después de cada cambio.

## Pregunta individual
**¿Qué parte de la rama de editar del user flow se modifica?**

Cambia el tramo «Editar cantidad → Recalcular total → Revisar» de la rama de editar: después de cada edición se recalcula y anuncia el total, y desde «Revisa y confirma» se agregó la decisión «¿El importe mostrado coincide con el total?»; si no coincide, regresa a revisar en lugar de enviar.

## Incidencia
«Recalcular el total y anunciar cada cambio; impedir confirmar un importe obsoleto» — En `renderReview()` el botón «Confirmar · $X» se actualiza en cada edición y `live()` anuncia «Total actualizado»; en el clic de confirmar se compara el importe mostrado con `total()` y, si difieren, se bloquea con «El total cambió». Ver `docs/incidencia.md`.
