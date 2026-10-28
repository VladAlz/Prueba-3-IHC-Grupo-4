# Defensa — IHC-A-10 · Dashboard UX · Stepper y checklist con lector de pantalla

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | Vinces Cueva Boris Yussef |
| Revisor del pull request y observador de la prueba | González Álvarez Vladimir Humberto |
| Issue del hallazgo | #10 |
| Ramas | `feature/boris-tarjetas-10-12` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-01:** `renderStepper()` escribe `#where` con «Paso n de 5 · Nombre» y agrega `aria-current` al paso actual.

**3. Mejora vinculada a la Issue #10:** `renderStepper()` muestra «Paso n de 5 · Nombre», ✓ en completados y texto oculto «(paso actual)/(completado)». Medición: 188 s / 3 errores → 129 s / 1 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó González Álvarez Vladimir Humberto, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar el texto de `#where` o el anuncio de `live()` en `go()`.

## Pregunta individual
**Demuestre cómo conoce el paso actual sin depender del color.**

Con NVDA: al llegar al Stepper se escucha «Participante, paso actual» (aria-current) y el texto «Paso 2 de 5 · Participante»; al pulsar Continuar se anuncia «Paso 3 de 5: Checklist previa» y el foco pasa al título. En escala de grises el paso se identifica igual (texto, número y ✓).
