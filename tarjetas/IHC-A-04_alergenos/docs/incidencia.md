# Incidencia — IHC-A-04 · CaféU · Advertencia de alérgenos antes de confirmar

| Campo | Detalle |
|---|---|
| Incidencia (minuto 100) | Incorporar aviso accesible y opción de volver a editar sin perder pedido |
| Responsable / revisor | Mora Beltrán Santiago Sebastián / Acaro Ibujés Pedro Sebastián |
| Requisito nuevo | **RF-07** — La advertencia es accesible (role="alert", recibe el foco al entrar) y ofrece «Volver a editar sin perder el pedido», que lleva al producto marcado. |
| Criterio | Al abrir «Revisa y confirma» el lector lee la advertencia; el enlace lleva a «Mi pedido» con el foco en «Quitar Brownie». |
| Flujo | `diagramas/user-flow.png` (nodos en naranja) |
| Cambio en el prototipo | El aviso tiene `role="alert"`, recibe el foco y ofrece «Volver a editar sin perder el pedido», que abre «Mi pedido» con el foco en el producto marcado. |
| Prueba | Usó «Volver a editar sin perder el pedido» y quitó el brownie; café y sánduche se conservaron — 84 s, 0 errores. Cita: «Me llevó directo al brownie.» |
| Commit | Rama `fix/santiago-incidencias-04-06`, posterior a la entrega, con «Closes #» de la issue de la incidencia |

| Antes (v2) | Después (v2 con incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
