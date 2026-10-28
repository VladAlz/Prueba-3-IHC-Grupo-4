# Defensa — IHC-A-11 · Dashboard UX · Jerarquía en 360 px sin superposiciones

| Rol | Integrante |
|---|---|
| Responsable de la tarjeta (todas las fases) | Vinces Cueva Boris Yussef |
| Revisor del pull request y observador de la prueba | González Álvarez Vladimir Humberto |
| Issue del hallazgo | #11 |
| Ramas | `feature/boris-tarjetas-10-12` |

**1. Ruta normal y de error:** ver `prototipo/README.md`.

**2. Requisito en el código — RF-02:** Las clases `.narrow`, `.compact` y el orden de `#actions` en el DOM definen el layout de 360 px.

**3. Mejora vinculada a la Issue #11:** Se quitan el margen negativo y la altura fija de `.card.step` (clase `bug`); los campos quedan visibles. Medición: 176 s / 3 errores → 121 s / 1 errores.

**4. Revisión cruzada:** el pull request de esta tarjeta lo revisó González Álvarez Vladimir Humberto, que comprobó las rutas normal y de error y la trazabilidad.

**5. Modificación breve en vivo:** Cambiar en CSS el ancho del Stepper compacto o el orden de un campo.

## Pregunta individual
**¿Qué ley Gestalt aplica y qué carga cognitiva se reduce?**

Región común (Gestalt): cada etapa vive en su propia card separada del Stepper, y proximidad para agrupar etiqueta y campo. Se reduce la carga cognitiva extrínseca: la persona ya no busca campos ocultos ni reconstruye qué paso está activo.
