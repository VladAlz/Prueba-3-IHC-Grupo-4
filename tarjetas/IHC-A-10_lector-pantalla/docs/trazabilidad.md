# Matriz de trazabilidad — IHC-A-10 · Dashboard UX · Stepper y checklist con lector de pantalla

**Responsable:** Vinces Cueva Boris Yussef

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Todas | Stepper | «Paso n de 5 · Nombre» | `wf-01-inicio` | prototipo/v2 · evidencias/antes-despues/ |
| RF-02 | Todas | Stepper | Ícono ✓ + texto oculto «completado» | `wf-01-inicio` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-03 | Principal: Paso 3 Checklist | Paso 3 Checklist | Contador anunciado | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-04 | Error / éxito | Todas | role="alert" / role="status" | `wf-03-error` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-01 | Todas | Todas | Texto + número + ícono (no solo color) | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Todas | Todas | Foco al título, foco visible, aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-01** y la restricción con **RF-04**.
