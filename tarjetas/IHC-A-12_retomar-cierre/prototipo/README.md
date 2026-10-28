# Guía de ejecución — IHC-A-12 · Dashboard UX · Retomar una prueba y cerrar sin éxito falso

| Versión | Enlace |
|---|---|
| v1 | https://raw.githack.com/VladAlz/Prueba-3-IHC-Grupo-4/main/tarjetas/IHC-A-12_retomar-cierre/prototipo/v1/index.html |
| v2 | https://raw.githack.com/VladAlz/Prueba-3-IHC-Grupo-4/main/tarjetas/IHC-A-12_retomar-cierre/prototipo/v2/index.html |

Sin internet: abrir `v1/index.html` o `v2/index.html` con doble clic.

| Parámetro | Uso |
|---|---|
| `?prueba=1` | Panel del moderador: provocar un fallo al guardar el cierre e interrumpir la sesión. |
| `?vista=wireframe` | Vista de baja fidelidad. |

**Ruta normal:** Plan (tarea) → Participante (P-07) → Checklist (3 obligatorios) → Registro («Agregar registro») → Revisión y cierre → «Finalizar sesión» → «Sesión finalizada».

**Ruta de error:** con `?prueba=1` activar «Fallo al guardar el cierre»; aparece el error con el foco en el mensaje y la opción de reintentar sin perder datos.

**Teclado:** Tab / Shift+Tab, Enter, Espacio; el primer Tab muestra «Saltar al contenido».
