# Matriz de trazabilidad — IHC-A-02 · CaféU · Editar y finalizar un pedido solo con teclado

**Responsable:** Acaro Ibujés Pedro Sebastián

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Principal: Menú → Agregar | 2.0 Menú de hoy | Botón «Agregar» + aviso + contador | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-02 | Editar: cambiar cantidad | 3.0 Mi pedido | Botones − / + y cantidad | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-03 | Editar: «¿Quitar X?» Sí / Cancelar | 3.0 Mi pedido | Botón «Quitar X del pedido» + diálogo | `wf-03-error` | prototipo/v2 · evidencias/antes-despues/ |
| RF-04 | Editar: Escape cancela / vuelve | 3.0 Mi pedido | Diálogo y botón «Volver» con Escape | `wf-03-error` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-01 | Todas | Todas | Foco de 3 px, «Saltar al contenido», aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Todas | Todas | Región aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| **RF-07** | Editar: quitar → foco al siguiente | 3.0 Mi pedido | Nombres accesibles de −, +, Quitar; foco restaurado | `wf-02-accion` | prototipo/v2 · evidencias/incidencia/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-03** y la restricción con **RNF-01**.
