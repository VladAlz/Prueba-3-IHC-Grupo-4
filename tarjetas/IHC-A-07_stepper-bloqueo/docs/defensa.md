# Defensa — IHC-A-07 · Dashboard UX · Stepper que no permite saltar etapas

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | González Álvarez Vladimir Humberto |
| Revisor del pull request y observador de la prueba | Mora Beltrán Santiago Sebastián |
| Issue del hallazgo | #7 · Issue de la incidencia (cerrada por el PR de incidencias) |
| Ramas | `feature/vladimir-tarjetas-07-09` · `fix/vladimir-incidencias-07-09` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-03:** `canVisit(i)` exige `complete(k)` de todas las etapas previas; `tryGo()` decide entre ir o explicar.

**3. Mejora vinculada a la Issue #7:** `canVisit()` bloquea etapas futuras (`aria-disabled`) y «Continuar» se deshabilita hasta cumplir `missing()`. Medición: 154 s / 2 errores → 131 s / 1 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó Mora Beltrán Santiago Sebastián, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar en `missing()` un requisito (por ejemplo, exigir 2 registros) o el texto de `explain()`.

## Pregunta individual
**¿Cómo aplica la visibilidad del estado del sistema de Nielsen?**

Con el Stepper (pasos completados ✓, actual resaltado y «Paso n de 5 · Nombre» en texto), la barra de progreso, el estado de guardado y mensajes inmediatos al intentar avanzar; la persona siempre sabe dónde está, qué terminó y qué falta.

## Incidencia
«Bloquear avances inválidos con explicación y permitir volver sin perder marcas» — `tryGo()` y «Continuar» llaman a `explain()`, que muestra la lista de faltantes con `role="alert"` y foco; las marcas se conservan al volver. Ver `docs/incidencia.md`.
