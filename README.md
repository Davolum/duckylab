# DuckyLab 🦆🧪

Creador de **cartas propias** de **Magic: The Gathering** y **Disney Lorcana**. Es una app aparte de DuckyCardVerse: aquí solo están las cartas que creas tú.

## Qué hace

- **Crear cartas** de Magic o de Lorcana con los botones «+ Carta Magic» y «+ Carta Lorcana».
- **Imagen**: súbela, arrástrala o pégala con Ctrl+V. Para encuadrarla, arrástrala sobre la carta y usa la rueda del ratón o la barra de zoom.
- **Datos de Magic**: nombre, coste de maná (con su propio editor: botones para añadir símbolos y, para quitar uno, se toca en la fila de arriba; «Vaciar» lo borra todo), línea de tipo, color del marco (automático según el coste o a mano), rareza, fuerza/resistencia, lealtad, ilustrador, set y número.
- **Datos de Lorcana**: nombre y versión, tipo (personaje, acción, canción, objeto, localización), clasificaciones, coste, tinta (y segunda tinta), si se puede usar como tinta, fuerza, voluntad, leyenda, coste de mover, rareza…
- **Texto con el lenguaje del juego** (botones de símbolos encima del texto):
  - Magic: `{T}` girar, `{Q}` enderezar, `{2}` `{X}`, `{W}{U}{B}{R}{G}`, `{C}`, híbridos `{W/U}`, pirexianos `{G/P}`, `{S}` nieve, `{E}` energía.
  - Lorcana: `{E}` agotar, `{I}` tinta, `{S}` fuerza, `{W}` voluntad, `{L}` leyenda.
  - `**negrita**`, `*cursiva*` y `~` (pone el nombre de la carta). Lo que va entre paréntesis sale en cursiva. La letra se encoge sola si el texto no cabe. Con retroceso se borra un símbolo `{…}` entero de una vez.
- **🎨 Estilo de arte**, con una miniatura en directo de cada opción:
  - Magic: Clásico, Arte extendido, Sin bordes, Arte completo, Vitrina ornamental, Antiguo y Solo arte.
  - Lorcana: Estándar, Arte completo, Encantada, Sin marco y Solo arte.
  - Color del borde: negro, blanco, plateado o dorado.
- **🖼 Plantillas** (botón de la cabecera): tus marcos con las posiciones de sus textos.
  - **Nueva plantilla**: subes la imagen de un marco (mejor PNG con el hueco del arte transparente; si el hueco es blanco, DuckyLab puede volverlo transparente).
  - **Duplicar** para hacer variantes, **renombrar**, **cambiar la imagen** manteniendo las posiciones y **borrar**. Cada plantilla muestra cuántas cartas la usan.
  - **Editor de plantillas**: pulsas cualquier texto de la carta y lo arrastras; con la rueda del ratón encima cambias su tamaño; también con la lista de elementos, las flechas (Mayús: de 10 en 10) o escribiendo el valor. Por elemento: **tipografía** (Barlow, Barlow Condensed, Cormorant Garamond, Libre Baskerville, EB Garamond, Cinzel, Oswald, Montserrat, Lora, Bebas Neue o una fuente instalada en tu ordenador), grosor, cursiva, mayúsculas, **color HEX**, alineación y mostrar u ocultar. Puedes previsualizarla con cualquiera de tus cartas.
  - En el **creador de cartas** eliges la plantilla en «🎨 Estilo de arte». «✏️ Editar plantilla» te lleva a su editor y te devuelve a la carta; «Hacer una variante solo para esta carta» la duplica para cambiarla sin tocar las demás.
  - Las plantillas se guardan en tu navegador y entran en la «💾 Copia».
- **🔤 Tipografía** (en el panel de estilo), por defecto **«Según tu guía»**:
  - Magic: nombre, línea de tipo y fuerza/resistencia en Cormorant Garamond (600–700); reglas en Libre Baskerville, con recordatorios y ambientación en cursiva.
  - Lorcana: nombre en Barlow Condensed SemiBold en mayúsculas; subtítulo y habilidades en Barlow Medium; encabezados de habilidad en Barlow Bold, que se ponen en mayúsculas solos; clasificaciones y ambientación en Barlow Italic; números en Barlow.
  - «Clásica DuckyLab» recupera EB Garamond y Cinzel. Los dorsos de DuckyLab siempre usan la clásica.
  - Las fuentes se descargan de Google Fonts la primera vez; después quedan guardadas para usarlas sin conexión.
- **✨ Efectos**: foil arcoíris, grabado metálico, purpurina, holográfico y galaxia. Se ven en la vista previa y salen al exportar e imprimir.
- **Voltear** la carta para ver el dorso: en el editor y en «Mis cartas» (botón ↻).
- **Dorso**: el diseño de DuckyLab, **«Mi dorso»** (una imagen que subes una vez por juego y que se usa en todas tus cartas de Magic o de Lorcana, incluidas las nuevas) o una imagen solo para una carta. Los dorsos oficiales no vienen incluidos porque son diseños de Wizards of the Coast y de Disney/Ravensburger. La imagen que subas la eliges tú.
- **Exportar** cada carta en **PNG** (con esquinas redondeadas), **JPG** o **PDF** a tamaño real: frente, dorso o las dos caras.
- **Imprimir varias**: pulsa «☑ Seleccionar», marca las cartas y pulsa «🖨 Imprimir». Crea un PDF con:
  - papel A4 o Carta, 9 cartas por hoja, o una carta por página;
  - copias de cada carta;
  - dorsos en páginas alternas, ya en espejo para imprimir a doble cara (dando la vuelta por el borde largo);
  - marcas de corte.
  - Al imprimir, elige **tamaño real / 100 %**, no «ajustar a la página». Cada carta mide 63 × 88 mm, como las de verdad.
- **💾 Copia**: descarga o restaura un archivo con todas tus cartas, tus dorsos y tus marcos guardados (imágenes incluidas).

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La app entera |
| `manifest.webmanifest`, `sw.js` | Permiten instalarla como app y abrirla sin conexión |
| `icon.svg`, `icon-192.png`, `icon-512.png` | Iconos |

## Publicarla gratis en GitHub Pages

DuckyLab no necesita descargar nada cada día, así que no lleva proceso automático.

1. En GitHub, crea un repositorio nuevo **Public**, por ejemplo `duckylab`.
2. **Add file → Upload files**, arrastra todos los archivos de la carpeta `duckylab` y pulsa **Commit changes**.
3. Ve a **Settings → Pages**. En «Build and deployment → Source» elige **Deploy from a branch**, rama **main** y carpeta **/ (root)**. Pulsa **Save**.
4. En un par de minutos estará en `https://TU-USUARIO.github.io/duckylab/`.

También funciona abriendo `index.html` con doble clic, pero así no se puede instalar como app.

## Instalarla como app

- **PC (Chrome o Edge)**: botón «⬇ Instalar» o el icono de instalar de la barra de direcciones.
- **Android**: menú ⋮ → «Instalar aplicación».
- **iPhone (Safari)**: Compartir → «Añadir a pantalla de inicio».

## ⚠️ Dónde se guardan las cartas

En el **navegador** de cada dispositivo, no en internet. Si se borran los datos del navegador, se pierden: haz una **💾 Copia** de vez en cuando. Para pasar las cartas a otro dispositivo, descarga la copia en uno y restáurala en el otro.

## Actualizar la app

Si cambias `index.html`, súbelo de nuevo y **sube también `sw.js` cambiando `VERSION`** (por ejemplo de `duckylab-v11` a `duckylab-v12`). Así el móvil coge la versión nueva. Las cartas guardadas no se tocan.

## Nota

App personal y no oficial. Los marcos, símbolos y dorsos son de diseño propio. No copian los oficiales. Magic: The Gathering © Wizards of the Coast. Disney Lorcana © Disney / Ravensburger.
