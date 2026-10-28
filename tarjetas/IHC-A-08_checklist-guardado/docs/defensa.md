# Defensa — IHC-A-08 · Dashboard UX · Checklist que se conserva y estado de guardado

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | González Álvarez Vladimir Humberto |
| Revisor del pull request y observador de la prueba | Mora Beltrán Santiago Sebastián |
| Issue del hallazgo | #8 |
| Ramas | `feature/vladimir-tarjetas-07-09` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-03:** `go()` cambia de etapa sin tocar `S.checks`; `step2()` pinta cada casilla con `S.checks[c.id]`.

**3. Mejora vinculada a la Issue #8:** `go()` ya no reinicia `S.checks`; el render de la etapa 3 lee el estado guardado. Medición: 166 s / 2 errores → 97 s / 0 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó Mora Beltrán Santiago Sebastián, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar el texto de `markSaved()` o el tiempo de guardado.

## Pregunta individual
**¿Qué evidencia muestra una mejora real frente a una mejora inferida?**

Mejora real: medida con la misma tarea y la misma persona — en v1 se observaron 2 errores y no finalizó (166 s); en v2 finalizó sin errores (97 s), con cita textual y capturas antes/después. Mejora inferida: lo que esperamos (por ejemplo, que el indicador «Guardado · hora» reduzca la ansiedad) sin una medición directa; se registra como estimada.
