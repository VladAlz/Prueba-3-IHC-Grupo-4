# Matriz de trazabilidad — IHC-A-07 · Dashboard UX · Stepper que no permite saltar etapas

**Responsable:** González Álvarez Vladimir Humberto

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Todas | Stepper | Stepper + «Paso n de 5» | `wf-01-inicio` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-02 | «¿Etapa actual completa?» | Pasos 1–4 | Validación por etapa | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-03 | «¿Etapa actual completa?» → bloqueo | Stepper | Pasos futuros con aria-disabled; Continuar | `wf-02-accion` | prototipo/v2 · evidencias/antes-despues/ |
| RF-04 | Editar: «Anterior» / «Editar» | Pasos 1–5 | Datos conservados | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-01 | Todas | Todas | Foco al título, foco visible, aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Cierre: Guardando → ¿Se guardó? → Finalizada / Error | Paso 5 · Sesión finalizada | Botón bloqueado, banner de error, código de sesión | `wf-04-confirmacion` | prototipo/v1 y v2 · evidencias/estados/ |
| **RF-07** | No completa → explicación | Paso actual | Banner role="alert" con la lista de faltantes | `wf-03-error` | prototipo/v2 · evidencias/incidencia/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-03** y la restricción con **RF-01**.
