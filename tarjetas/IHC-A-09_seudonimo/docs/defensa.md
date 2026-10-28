# Defensa — IHC-A-09 · Dashboard UX · Participantes anónimos con código seudónimo

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | González Álvarez Vladimir Humberto |
| Revisor del pull request y observador de la prueba | Mora Beltrán Santiago Sebastián |
| Issue del hallazgo | #9 · Issue de la incidencia (cerrada por el PR de incidencias) |
| Ramas | `feature/vladimir-tarjetas-07-09` · `fix/vladimir-incidencias-07-09` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RNF-01:** `step1()` solo crea el campo `#pid`; `rowsTable()` usa `S.pid` y nunca un nombre.

**3. Mejora vinculada a la Issue #9:** `step1()` reemplaza el nombre por «Código de participante»; `rowsTable()` y el resumen muestran solo el código. Medición: 139 s / 2 errores → 88 s / 0 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó Mora Beltrán Santiago Sebastián, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar la expresión regular de `missing(1)` (por ejemplo, aceptar 4 dígitos) o el texto de la pista.

## Pregunta individual
**¿Qué requisito protege privacidad y dónde aparece en la trazabilidad?**

RNF-01 (privacidad) y RF-07 (formato del código). En docs/trazabilidad.md, RNF-01 → flujo «Registrar participante» → pantalla Participante → componente campo «Código» → wireframe 02 (acción); RF-07 → rama de error «Código inválido» → wireframe 03 (error).

## Incidencia
«Sustituir por código seudónimo y validar su formato» — `missing(1)` valida `/^P-\d{2,3}$/`; `fieldErr()` muestra el error junto al campo con `aria-invalid` y `aria-describedby`. Ver `docs/incidencia.md`.
