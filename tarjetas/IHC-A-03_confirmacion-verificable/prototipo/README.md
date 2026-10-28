# Guía de ejecución — IHC-A-03 · CaféU · Confirmación verificable en un dispositivo compartido

| Versión | Enlace |
|---|---|
| v1 | https://raw.githack.com/VladAlz/Prueba-3-IHC-Grupo-4/main/tarjetas/IHC-A-03_confirmacion-verificable/prototipo/v1/index.html |
| v2 | https://raw.githack.com/VladAlz/Prueba-3-IHC-Grupo-4/main/tarjetas/IHC-A-03_confirmacion-verificable/prototipo/v2/index.html |

Sin internet: abrir `v1/index.html` o `v2/index.html` con doble clic.

| Parámetro | Uso |
|---|---|
| `?prueba=1` | Panel del moderador: provocar un fallo de red. |
| `?vista=wireframe` | Vista de baja fidelidad. |

**Ruta normal:** «Ver menú» → «Agregar» café y sánduche → «Mi pedido» (− / +) → «Revisar pedido» → «Confirmar» → «Enviando…» → confirmación con número.

**Ruta de error:** con `?prueba=1` activar «Fallo de red en el próximo envío»; aparece el error con el foco en el mensaje y la opción de reintentar sin perder datos.

**Teclado:** Tab / Shift+Tab, Enter, Espacio, Escape; el primer Tab muestra «Saltar al contenido».
