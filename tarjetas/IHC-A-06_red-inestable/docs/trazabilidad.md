# Matriz de trazabilidad — IHC-A-06 · CaféU · Confirmación sin duplicados con red inestable

**Responsable:** Mora Beltrán Santiago Sebastián

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Principal: Revisa y confirma | 3.1 Revisa y confirma | Resumen y total | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-02 | Principal: Confirmar → Procesando | 3.1 Revisa y confirma | Botón bloqueado (aria-busy) | `wf-02-accion` | prototipo/v2 · evidencias/antes-despues/ |
| RF-03 | Principal: Procesando | 3.1 Revisa y confirma | «Enviando…» con barra, sin éxito | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-04 | Error: «¿Respondió?» → Reintentar | 3.1 Revisa y confirma | Banner de error + «Reintentar envío» | `wf-03-error` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-01 | Error | 3.1 Revisa y confirma | Carrito conservado tras el error | `wf-03-error` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Todas | Todas | Foco de 3 px, «Saltar al contenido», aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| **RF-07** | Pendiente / Confirmado / No confirmado | 3.1 · 4.0 | Chips de estado + código de envío | `wf-03-error` | prototipo/v2 · evidencias/incidencia/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-02** y la restricción con **RNF-01**.
