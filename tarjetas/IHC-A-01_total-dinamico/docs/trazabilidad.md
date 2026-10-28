# Matriz de trazabilidad — IHC-A-01 · CaféU · Total que se actualiza en un pedido rápido

**Responsable:** Acaro Ibujés Pedro Sebastián

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Principal: Menú → Agregar | 2.0 Menú de hoy | Botón «Agregar» + aviso + contador | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-02 | Editar: cambiar cantidad | 3.0 Mi pedido | Botones − / + y cantidad | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-03 | Editar: cantidad → recalcular total | 3.0 Mi pedido | Subtotal, fila Total y botón «Revisar pedido · $X» | `wf-02-accion` | prototipo/v2 · evidencias/antes-despues/ |
| RF-04 | Principal: Procesando → ¿Respondió? → Éxito / Error | 3.1 Revisa y confirma · 4.0 | Botón Confirmar bloqueado, banner de error, tarjeta de éxito | `wf-03-error` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-01 | Todas (tiempo < 3 min) | Todas a 360 px | Layout de una columna y botón principal fijo | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Todas | Todas | Foco de 3 px, «Saltar al contenido», aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-03** y la restricción con **RNF-01**.
