# Intiyachay — prototipo rediseñado

Versión del 19 de octubre de 2026, preparada a partir de INTIYACHAY.zip. Sitio con interacciones en JavaScript y alojamiento estático HTML/CSS; fotografías locales y sin instalación de dependencias. No es un tema instalable de WordPress ni una aplicación Next.js.

## Abrir localmente

Desde esta carpeta:

```sh
python3 -m http.server 4173
```

Abre http://localhost:4173. Utiliza un servidor: las rutas absolutas de recursos y navegación no están pensadas para abrir el HTML por doble clic.

## Publicar en Vercel

Sube el contenido de esta carpeta a la raíz de un repositorio e impórtalo en Vercel. Selecciona un proyecto estático / Other, sin comando de compilación ni instalación; usa la raíz del proyecto como directorio de salida. Se incluye vercel.json con rutas y redirecciones.

No se ha publicado en ninguna cuenta. Las etiquetas noindex, robots.txt y la cabecera X-Robots-Tag impiden solicitar indexación del prototipo. Antes de publicar la versión definitiva, retirar esas tres restricciones según el alcance aprobado.

## Pantallas

- / — Inicio.
- /modelo-educativo/ — Modelo educativo.
- /oferta-educativa/ — Niveles educativos, nueva página que organiza contenido existente.
- /nuestras-instalciones/ — Instalaciones y galería. Se conserva la ruta original aunque su escritura contenga un error; el texto visible está corregido.
- /acerca-de-nosotros/ — Nosotros.
- /contacto/ — Correo, ubicación y horario publicado.

En Vercel, /instalaciones y /nosotros redirigen a las rutas originales correspondientes.

## Diseño y colores

Todos estos valores se encontraron en HTML/CSS del ZIP original:

- #7ABB3B — verde institucional, botones y detalles.
- #1B3D22 — verde oscuro ya presente en modelo-educativo/index.html; titulares y pie.
- #F4F6F5 — fondo claro ya presente en modelo-educativo/index.html.
- #FFFFFF — blanco.
- #353535 — texto.
- #4A5568 — texto secundario, presente en modelo educativo.
- #E5E5E5 — separadores.
- #16B7CC — acento original conservado como variable disponible.

El rediseño selecciona y organiza colores existentes; no usa los colores complementarios nuevos del prompt anterior. La tipografía usa Georgia y Arial con fuentes del sistema para no depender de descargas externas.

## Editar

- Contenido: index.html dentro de cada ruta.
- Estilos y diseño responsivo: assets/styles.css.
- Menú, galería, consultas por nivel y año: assets/site.js.
- Fotos, dimensiones y URL de procedencia: assets/imagenes.json.

Logo y fotografías se copiaron del ZIP aportado. Las fotos históricas no se presentan como eventos actuales. Los originales no se modificaron.

## Comportamiento

- Menú móvil desplegable, cierre con Escape y cierre al navegar.
- Cuatro niveles en acordeones; el enlace con fragmento abre el nivel elegido.
- Galería con filtros y visor modal; cierre con Escape y navegación con flechas.
- Contacto mediante mailto. El visitante envía desde su aplicación de correo; no se afirma que el prototipo haya enviado información.
- Mapa abre el destino original en Google Maps.
- Año dinámico en zona horaria America/Guayaquil.

Moodle, tienda, cuentas y formularios sin funcionamiento verificado están excluidos, conforme al alcance acordado. Se omite el teléfono de formato dudoso. Los anuncios antiguos de matrícula se sustituyeron por consultas de información, sin inventar fechas o disponibilidad.

## Actualización interactiva

- Logo como botón de inicio con esquinas redondeadas, relieve y respuesta al pulsar.
- Hero con vídeo original, portada fotográfica, reproducción, pausa y control de sonido.
- El vídeo se carga al pulsar reproducir; no se reproduce audio automáticamente.
- Selector Comunidad / Naturaleza / Creatividad con fotografías originales y flechas anterior/siguiente.
- Mapa Google Maps incrustado en Inicio y Contacto, con ubicación recuperada de la portada original del ZIP.
- Aparición progresiva de contenido, estados hover/foco y respeto de movimiento reducido.
- Tipografía sans serif y componentes más redondeados en todas las páginas.

El ZIP original enlaza el vídeo, pero no contiene el archivo. El reproductor usa la URL original guardada en assets/video-origen.txt; requiere conexión y depende de la disponibilidad del servidor de Intiyachay. El mapa también requiere conexión. No se descargó el vídeo en esta actualización.

Para revisar el vídeo y el mapa, inicia el servidor local indicado arriba o despliega en Vercel. Esta actualización pasó comprobación de sintaxis de JavaScript, referencias locales y colores; no se pudo hacer una nueva prueba visual en navegador debido a las restricciones del entorno.
