# Matriz de trazabilidad — IHC-A-09 · Dashboard UX · Participantes anónimos con código seudónimo

**Responsable:** González Álvarez Vladimir Humberto

Requisito → flujo → pantalla → componente → wireframe → prototipo/evidencia.

| Requisito | Flujo (nodo / rama) | Pantalla | Componente | Wireframe | Prototipo y evidencia |
|---|---|---|---|---|---|
| RF-01 | Principal: Paso 2 Participante | Paso 2 Participante | Campo «Código de participante» | `wf-02-accion` | prototipo/v2 · evidencias/antes-despues/ |
| RF-02 | Principal: Paso 4 Registro | Paso 4 Registro | Formulario y tabla de registros | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-03 | Pasos 4–5 y cierre | Tabla, resumen, confirmación | Columna «Código» (sin nombres) | `wf-04-confirmacion` | prototipo/v1 y v2 · evidencias/estados/ |
| RF-04 | Cierre: Guardando → ¿Se guardó? → Finalizada / Error | Paso 5 · Sesión finalizada | Botón bloqueado, banner de error, código de sesión | `wf-04-confirmacion` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-01 | Paso 2 Participante | Paso 2 | Sin campo de nombre; pista «No escribas nombres» | `wf-02-accion` | prototipo/v1 y v2 · evidencias/estados/ |
| RNF-02 | Todas | Todas | Foco al título, foco visible, aria-live | `wf-01 a wf-04` | prototipo/v1 y v2 · evidencias/estados/ |
| **RF-07** | «¿Formato P-07?» → error | Paso 2 Participante | Error junto al campo (aria-invalid) | `wf-03-error` | prototipo/v2 · evidencias/incidencia/ |

Sitemap: `diagramas/sitemap.png` · User flow: `diagramas/user-flow.png` · Wireframes: `wireframes/`. El fallo de la tarjeta se cubre con **RF-01** y la restricción con **RNF-01**.
