# Fase 2 · Requisitos verificables — IHC-A-07 · Dashboard UX · Stepper que no permite saltar etapas

**Responsable:** González Álvarez Vladimir Humberto

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Mostrar el Stepper de 5 etapas con el paso actual en texto («Paso n de 5»). | El texto cambia en cada etapa. | Restricción de la tarjeta |
| RF-02 | Definir requisitos por etapa (tarea, código, obligatorios de checklist, ≥1 registro). | `missing(i)` devuelve la lista por etapa. | Tarea crítica |
| RF-03 | Impedir avanzar a una etapa futura si la actual no está completa. | En v2 los pasos futuros quedan bloqueados. | Fallo de la tarjeta (Issue #7) |
| RF-04 | Permitir volver a etapas anteriores conservando los datos. | Al volver al paso 3, las marcas siguen. | Tarea crítica |
| RNF-01 | Operable con teclado; foco al título de cada etapa. | Tab recorre la etapa; el foco va al título. | Tarea crítica |
| RNF-02 | Estados del cierre: procesando, error y éxito. | Se ven los tres estados. | Accesibilidad (WCAG 2.2) |
