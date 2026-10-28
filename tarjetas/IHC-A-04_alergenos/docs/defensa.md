# Defensa — IHC-A-04 · CaféU · Advertencia de alérgenos antes de confirmar

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | Mora Beltrán Santiago Sebastián |
| Revisor del pull request y observador de la prueba | Acaro Ibujés Pedro Sebastián |
| Issue del hallazgo | #4 · Issue de la incidencia (cerrada por el PR de incidencias) |
| Ramas | `feature/santiago-tarjetas-04-06` · `fix/santiago-incidencias-04-06` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-04:** En el clic de `#confirm` se revisa `flaggedInCart()` y `#alerg-ok`; si falta la casilla se muestra `#alerg-err` y se enfoca la casilla.

**3. Mejora vinculada a la Issue #4:** Etiqueta «⚠ Contiene…» en menú y pedido; en `renderReview()` aviso y casilla obligatoria; el clic de confirmar valida la casilla. Medición: 118 s / 1 errores → 97 s / 0 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó Acaro Ibujés Pedro Sebastián, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar el texto de la advertencia o el destino del foco del enlace «Volver a editar».

## Pregunta individual
**¿Cómo prueba que el usuario comprende y puede corregir su elección?**

Con dos evidencias observadas: (1) comprensión — en la prueba la persona verbaliza «el brownie tiene nueces» al leer el aviso; (2) corrección — usa «Volver a editar», quita el brownie y confirma solo café y sánduche (registro en pruebas/sesion.md, tiempo y cita).

## Incidencia
«Incorporar aviso accesible y opción de volver a editar sin perder pedido» — El aviso tiene `role="alert"`, recibe el foco y ofrece «Volver a editar sin perder el pedido», que abre «Mi pedido» con el foco en el producto marcado. Ver `docs/incidencia.md`.
