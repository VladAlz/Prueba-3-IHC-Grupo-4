# Defensa — IHC-A-12 · Dashboard UX · Retomar una prueba y cerrar sin éxito falso

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | Vinces Cueva Boris Yussef |
| Revisor del pull request y observador de la prueba | González Álvarez Vladimir Humberto |
| Issue del hallazgo | #12 · Issue de la incidencia (cerrada por el PR de incidencias) |
| Ramas | `feature/boris-tarjetas-10-12` · `fix/boris-incidencias-10-12` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-03:** `finish()` llama a `allOk()`, que exige `complete()` de las etapas 0–3; si falla, no llama a `done()`.

**3. Mejora vinculada a la Issue #12:** `finish()` revisa `allOk()` y, si falta algo, muestra el error con enlace al paso pendiente. Medición: 118 s / 1 errores → 104 s / 0 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó González Álvarez Vladimir Humberto, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar en `CHK` qué ítems son obligatorios o el texto del estado global de la revisión.

## Pregunta individual
**¿Cómo muestra el momento de verdad y comprueba el estado final?**

El momento de verdad es «Revisar y finalizar»: la revisión previa lo hace visible con ✓/✕ por cada obligatorio y un estado global («Aún no se puede cerrar» / «Todo listo»). El estado final se comprueba con el resumen de cierre (obligatorios 3 de 3, registros, código de sesión) y en la prueba con la observación de que ya no aparece éxito con pendientes.

## Incidencia
«Añadir revisión previa y resumen comprobable; evitar éxito falso» — `step4()` muestra la revisión previa ✓/✕ por punto; «Finalizar» se deshabilita (`aria-describedby`) mientras haya ✕; `done()` muestra un resumen comprobable con conteos. Ver `docs/incidencia.md`.
