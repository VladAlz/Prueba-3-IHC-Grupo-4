# Matriz de trazabilidad — IHC-A-04 · CaféU · Advertencia de alérgenos antes de confirmar

**Responsable:** Mora Beltrán Santiago Sebastián

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Principal: Inicio | 1.0 Inicio | Selector de alergia | `wf-01-inicio` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-02 | Principal: Menú → Info | 2.1 Detalle | Ingredientes y advertencia | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-03 | Principal: «¿Contiene su alérgeno?» | 2.0 Menú · 3.0 Mi pedido | Etiqueta «⚠ Contiene …» | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-04 | Error: «¿Leyó la advertencia?» | 3.1 Revisa y confirma | Advertencia + casilla obligatoria + error | `wf-03-error` | prototipo/v2 · evidencias/antes-despues/ |
| RNF-01 | Todas | Todas | Ícono + texto (no solo color) | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Todas | Todas | Foco de 3 px, «Saltar al contenido», aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-04** y la restricción con **RNF-01**.
