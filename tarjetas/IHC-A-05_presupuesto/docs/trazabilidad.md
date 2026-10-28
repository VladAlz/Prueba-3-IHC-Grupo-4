# Matriz de trazabilidad — IHC-A-05 · CaféU · Pedido dentro de un presupuesto de USD 4,25

**Responsable:** Mora Beltrán Santiago Sebastián

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Principal: Inicio → Menú | 1.0 Inicio · 2.0 Menú | Presupuesto y medidor «Llevas $X de $4,25» | `wf-01-inicio` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-02 | Editar: cambiar cantidad | 3.0 Mi pedido | Botones − / + y cantidad | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-03 | Editar: «¿Total supera $4,25?» | 3.0 Mi pedido | Medidor + aviso «Te pasas por $X» | `wf-03-error` | prototipo/v2 · evidencias/antes-despues/ |
| RF-04 | Principal: Procesando → ¿Respondió? → Éxito / Error | 3.1 Revisa y confirma · 4.0 | Botón Confirmar bloqueado, banner de error, tarjeta de éxito | `wf-03-error` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-01 | Editar | 3.0 Mi pedido | Aviso con ícono y texto | `wf-03-error` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Todas | Todas | Foco de 3 px, «Saltar al contenido», aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| **RF-07** | Confirmar: «¿Supera el presupuesto?» | 3.1 Revisa y confirma | Diálogo «Ajustar pedido» / «Confirmar igual» | `wf-03-error` | prototipo/v2 · evidencias/incidencia/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-03** y la restricción con **RNF-01**.
