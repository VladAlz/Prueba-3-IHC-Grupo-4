# Matriz de trazabilidad — IHC-A-08 · Dashboard UX · Checklist que se conserva y estado de guardado

**Responsable:** González Álvarez Vladimir Humberto

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Principal: Paso 1 Plan | Paso 1 Plan | Card «Cómo funciona esta sesión» | `wf-01-inicio` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-02 | Principal: Paso 3 Checklist | Paso 3 Checklist | Grid de casillas con Obligatorio/Opcional | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-03 | Cambio de etapa | Paso 3 Checklist | Estado de casillas conservado | `wf-02-accion` | prototipo/v2 · evidencias/antes-despues/ |
| RF-04 | Principal: Paso 3 Checklist | Paso 3 Checklist | Contador «n de 5 · n de 3» | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-01 | Todas | Todas | Foco al título, foco visible, aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Cierre: Guardando → ¿Se guardó? → Finalizada / Error | Paso 5 · Sesión finalizada | Botón bloqueado, banner de error, código de sesión | `wf-04-confirmacion` | prototipo/v1 y v2 · evidencias/estados/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-03** y la restricción con **RF-01**.
