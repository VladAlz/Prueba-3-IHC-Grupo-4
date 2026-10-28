# Decisiones de diseño y prototipado — IHC-A-11 · Dashboard UX · Jerarquía en 360 px sin superposiciones

**Responsable:** Vinces Cueva Boris Yussef

| Decisión | Justificación |
|---|---|
| Fidelidad media: navegable, con datos y estados reales. | La prueba requiere escribir, editar y ver procesando/error/éxito. |
| HTML + CSS + JavaScript en un archivo por versión. | Se abre sin instalar nada y permite teclado, foco, `aria-live` y validaciones reales. |
| Vista de baja fidelidad con `?vista=wireframe`. | Wireframes y prototipo salen del mismo código. |
| Panel del moderador con `?prueba=1`. | Permite provocar el error de red/guardado durante la prueba. |
| v1 como línea base del comportamiento de referencia. | La prueba observa el fallo («Card UI se superpone al Stepper y oculta campos») y la mejora de v2 queda medida, no supuesta. |

| Elemento | Decisión | Principio |
|---|---|---|
| Acción principal | Un botón principal por pantalla, abajo. | Jerarquía; Fitts |
| Agrupación | Cards por bloque. | Gestalt: región común y proximidad |
| Progreso | Stepper «Paso n de 5» con ✓. | N1 Visibilidad del estado |
| Estados | Procesando, error con salida, éxito con evidencia. | N1, N9 |
| Edición / cancelación | «Anterior» y «Editar» por etapa. | N3 Control y libertad |
| Teclado y foco | «Saltar al contenido», foco al título, anillo de 3 px. | WCAG 2.1.1, 2.4.3, 2.4.7 |
| Principio complementario | User flow de CaféU: una acción principal clara al final de cada pantalla. | Sax300-cpu/HCI-2026-G2 (CaféU y su carpeta presentacion) |
