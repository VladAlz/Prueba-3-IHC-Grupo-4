# Matriz de trazabilidad — IHC-A-12 · Dashboard UX · Retomar una prueba y cerrar sin éxito falso

**Responsable:** Vinces Cueva Boris Yussef

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Inicio: «¿Prueba interrumpida?» | Inicio | Guardado local del avance | `wf-01-inicio` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-02 | Inicio → aviso | Aviso de prueba retomada | Banner con pasos recuperados | `wf-01-inicio` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-03 | «¿Obligatorios completos?» → error | Paso 5 Revisión y cierre | Error con «Ir a…» | `wf-03-error` | prototipo/v2 · evidencias/antes-despues/ |
| RF-04 | Cierre: Guardando → ¿Se guardó? → Finalizada / Error | Paso 5 · Sesión finalizada | Botón bloqueado, banner de error, código de sesión | `wf-04-confirmacion` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-01 | Todas | Todas | Almacenamiento local | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Todas | Todas | Foco al título, foco visible, aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| **RF-07** | Revisión previa ✓/✕ | Paso 5 Revisión y cierre | Lista ✓/✕ + Finalizar deshabilitado | `wf-03-error` | prototipo/v2 · evidencias/incidencia/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-03** y la restricción con **RNF-01**.
