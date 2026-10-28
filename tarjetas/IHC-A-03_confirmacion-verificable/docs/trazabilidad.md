# Matriz de trazabilidad — IHC-A-03 · CaféU · Confirmación verificable en un dispositivo compartido

**Responsable:** Acaro Ibujés Pedro Sebastián

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Principal: Menú → Revisa | 3.1 Revisa y confirma | Resumen y total | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-02 | Principal: Procesando (sin éxito aún) | 3.1 Revisa y confirma | Botón bloqueado + barra «Enviando…» | `wf-03-error` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-03 | Principal: Éxito | 4.0 Confirmación | Número, resumen y total | `wf-04-confirmacion` | prototipo/v2 · evidencias/antes-despues/ |
| RF-04 | Principal: Éxito → Salir | 4.0 Confirmación | Botón «Salir y borrar este pedido» | `wf-04-confirmacion` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-01 | Todas | 1.0 Inicio · 4.0 | Aviso «Sin datos personales»; sin campos personales | `wf-01-inicio` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Todas | Todas | Foco de 3 px, «Saltar al contenido», aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-03** y la restricción con **RNF-01**.
