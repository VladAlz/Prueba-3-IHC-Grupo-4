# Incidencia — IHC-A-06 · CaféU · Confirmación sin duplicados con red inestable

| Campo | Detalle |
|---|---|
| Incidencia (minuto 100) | Modelar pendiente / confirmado / no confirmado y evitar duplicación |
| Responsable / revisor | Mora Beltrán Santiago Sebastián / Acaro Ibujés Pedro Sebastián |
| Requisito nuevo | **RF-07** — Modelar tres estados — Pendiente (◷, ámbar), Confirmado (✓, verde) y No confirmado (✕, rojo) — con texto, ícono y anuncio; reintentar usa el mismo código de envío para no duplicar. |
| Criterio | Con «Se corta», aparece «No confirmado»; al reintentar se obtiene un solo pedido N.º 031. |
| Flujo | `diagramas/user-flow.png` (nodos en naranja) |
| Cambio en el prototipo | `send()` asigna un código de envío `S.key` reutilizado al reintentar; la cafetería devuelve el mismo pedido si el código ya existe; los estados Pendiente / Confirmado / No confirmado tienen ícono, texto y anuncio propios. |
| Prueba | Con corte de red vio «No confirmado», reintentó y obtuvo un solo pedido — 73 s, 0 errores. Cita: «Dice que no se registró y que no se duplica, entonces reintento.» |
| Commit | Rama `fix/santiago-incidencias-04-06`, posterior a la entrega, con «Closes #» de la issue de la incidencia |

| Antes (v2) | Después (v2 con incidencia) |
|---|---|
| ![Antes](../evidencias/incidencia/antes-v2.png) | ![Después](../evidencias/incidencia/despues-v2-incidencia.png) |
