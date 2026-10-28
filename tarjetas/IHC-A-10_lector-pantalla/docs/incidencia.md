# Incidencia — IHC-A-10 · Dashboard UX · Stepper y checklist con lector de pantalla

| Campo | Detalle |
|---|---|
| Incidencia (minuto 100) | Añadir texto/estado accesible del paso activo y foco visible |
| Responsable / revisor | Vinces Cueva Boris Yussef / González Álvarez Vladimir Humberto |
| Requisito nuevo | **RF-07** — Paso activo con `aria-current="step"`, anuncio «Paso n de 5: Nombre» en cada cambio y foco visible de 3 px. |
| Criterio | NVDA lee «Participante, paso actual»; el anillo de foco es visible. |
| Flujo | `diagramas/user-flow.png` (nodos en naranja) |
| Cambio en el prototipo | `aria-current="step"`, `live()` anuncia «Paso n de 5: Nombre» en `go()`, foco al título y anillo de foco de 3 px. |
| Prueba | Se anunció cada cambio de paso y el foco quedó visible — 104 s, 0 errores. Cita: «Me avisa al cambiar, perfecto.» |
| Commit | Rama `fix/boris-incidencias-10-12`, posterior a la entrega, con «Closes #» de la issue de la incidencia |

| Antes (v2) | Después (v2 con incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
