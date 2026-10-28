# Defensa — IHC-A-03 · CaféU · Confirmación verificable en un dispositivo compartido

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | Acaro Ibujés Pedro Sebastián |
| Revisor del pull request y observador de la prueba | Vinces Cueva Boris Yussef |
| Issue del hallazgo | #3 |
| Ramas | `feature/pedro-tarjetas-01-03` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-03:** `send()` espera la respuesta antes de llamar a `success()`; `renderOk()` construye número/código, resumen y total.

**3. Mejora vinculada a la Issue #3:** `renderOk()` muestra «¡Pedido confirmado!», N.º de pedido, resumen y total en lugar de solo «Listo». Medición: 96 s / 1 errores → 71 s / 0 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó Vinces Cueva Boris Yussef, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar en `renderOk()` el texto del estado o el formato del código de retiro.

## Pregunta individual
**¿Cómo evita confundir clic efectuado con pedido confirmado?**

Separando tres estados: el clic solo inicia «Enviando…» (botón bloqueado, barra, sin palabras de éxito); el éxito solo aparece cuando llega la respuesta y siempre con evidencia verificable (código, desglose y «Recibido por la cafetería»). Un clic efectuado nunca muestra «Listo».
