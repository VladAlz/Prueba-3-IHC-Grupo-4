# Decisiones de diseño y prototipado — IHC-A-03 · CaféU · Confirmación verificable en un dispositivo compartido

**Responsable:** Acaro Ibujés Pedro Sebastián

| Decisión | Justificación |
|---|---|
| Fidelidad media: navegable, con datos y estados reales. | La prueba requiere escribir, editar y ver procesando/error/éxito. |
| HTML + CSS + JavaScript en un archivo por versión. | Se abre sin instalar nada y permite teclado, foco, `aria-live` y validaciones reales. |
| Vista de baja fidelidad con `?vista=wireframe`. | Wireframes y prototipo salen del mismo código. |
| Panel del moderador con `?prueba=1`. | Permite provocar el error de red/guardado durante la prueba. |
| v1 como línea base del comportamiento de referencia. | La prueba observa el fallo («La pantalla dice «Listo» pero no muestra número ni resumen») y la mejora de v2 queda medida, no supuesta. |

| Elemento | Decisión | Principio |
|---|---|---|
| Acción principal | Un botón principal por pantalla, abajo. | Jerarquía; Fitts |
| Agrupación | Cards por bloque. | Gestalt: región común y proximidad |
| Progreso | «Paso n de 3». | N1 Visibilidad del estado |
| Estados | Procesando, error con salida, éxito con evidencia. | N1, N9 |
| Edición / cancelación | «Editar pedido», «Seguir agregando», Escape. | N3 Control y libertad |
| Teclado y foco | «Saltar al contenido», foco al título, anillo de 3 px. | WCAG 2.1.1, 2.4.3, 2.4.7 |
| Principio complementario | Momentos de verdad y curva emocional del Dashboard UX aplicados a la confirmación. | maribelsailema/HCI_2026_G1 (Dashboard UX) |
