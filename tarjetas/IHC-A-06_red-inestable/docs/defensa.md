# Defensa — IHC-A-06 · CaféU · Confirmación sin duplicados con red inestable

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | Mora Beltrán Santiago Sebastián |
| Revisor del pull request y observador de la prueba | Acaro Ibujés Pedro Sebastián |
| Issue del hallazgo | #6 · Issue de la incidencia (cerrada por el PR de incidencias) |
| Ramas | `feature/santiago-tarjetas-04-06` · `fix/santiago-incidencias-04-06` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-02:** `send()` pone `S.busy = true`, deshabilita el botón y solo lo libera al recibir respuesta o error.

**3. Mejora vinculada a la Issue #6:** En `send()` el botón se deshabilita con `aria-busy` y spinner; `#confirm` ignora clics mientras `S.busy`. Medición: 64 s / 1 errores → 58 s / 0 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó Acaro Ibujés Pedro Sebastián, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar el texto o el ícono de un estado en `send()` o el tiempo de la red lenta.

## Pregunta individual
**¿Cómo diferencia visualmente y semánticamente los tres estados?**

Visualmente: Pendiente = chip ámbar con ◷ «Pendiente de confirmación»; Confirmado = chip verde con ✓; No confirmado = banner rojo con ✕; nunca solo color. Semánticamente: Pendiente usa `role="status"` y `aria-busy` en el botón; No confirmado usa `role="alert"` y recibe el foco; Confirmado se anuncia con el número de pedido.

## Incidencia
«Modelar pendiente / confirmado / no confirmado y evitar duplicación» — `send()` asigna un código de envío `S.key` reutilizado al reintentar; la cafetería devuelve el mismo pedido si el código ya existe; los estados Pendiente / Confirmado / No confirmado tienen ícono, texto y anuncio propios. Ver `docs/incidencia.md`.
