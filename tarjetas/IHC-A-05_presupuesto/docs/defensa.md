# Defensa — IHC-A-05 · CaféU · Pedido dentro de un presupuesto de USD 4,25

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | Mora Beltrán Santiago Sebastián |
| Revisor del pull request y observador de la prueba | Acaro Ibujés Pedro Sebastián |
| Issue del hallazgo | #5 |
| Ramas | `feature/santiago-tarjetas-04-06` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-03:** `changeQty()` vuelve a llamar a `renderCart()`, que con `budgetBox()` compara `total()` con `BUDGET` y muestra la diferencia.

**3. Mejora vinculada a la Issue #5:** `budgetBox()` se pinta en «Mi pedido» y «Revisa y confirma» con medidor y «Te pasas por $X» al editar. Medición: 109 s / 1 errores → 86 s / 0 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó Acaro Ibujés Pedro Sebastián, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar el texto del aviso de `budgetBox()` o el monto del presupuesto (`BUDGET`).

## Pregunta individual
**¿Qué touchpoint pasa a ser momento de verdad y por qué?**

«Editar Mi pedido» pasa a ser momento de verdad: en el diagnóstico se consideraba un paso neutro, pero la observación mostró que un solo «+» lleva el pedido de $4,25 a $5,75 sin aviso; ahí se decide si la persona respeta su presupuesto o paga de más (emoción −2 en la curva inicial).
