# Incidencia — IHC-A-11 · Dashboard UX · Jerarquía en 360 px sin superposiciones

| Campo | Detalle |
|---|---|
| Incidencia (minuto 100) | Reorganizar layout responsivo y conservar orden lógico del foco |
| Responsable / revisor | Vinces Cueva Boris Yussef / González Álvarez Vladimir Humberto |
| Requisito nuevo | **RF-07** — Layout responsivo de una columna con Stepper compacto, acciones fijas al final y orden del DOM = orden visual. |
| Criterio | En 360 px Tab va de los campos a Anterior/Continuar. |
| Flujo | `diagramas/user-flow.png` (nodos en naranja) |
| Cambio en el prototipo | Clase `compact`: Stepper compacto, una columna, acciones `sticky` al final y el DOM de acciones después de `main` para que el foco siga el orden visual. |
| Prueba | Stepper compacto, campos en orden y acciones al final — 98 s, 0 errores. Cita: «Ahora va en orden.» |
| Commit | Rama `fix/boris-incidencias-10-12`, posterior a la entrega, con «Closes #» de la issue de la incidencia |

| Antes (v2) | Después (v2 con incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
