<p align="center"></p>
<p align="center"><a href="#"><img width="115px" src="docs/assets/Logo-115px.png" align="center" alt="Drop Icons"/></a></p>
<h1 align="center">Drop Icons</h1>
<p align="center">Drop Icons es una aplicación para convertir imágenes a iconos (.ico) para Windows, con una función simple de arrastrar y soltar.</p>

<p align="center">
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/badge/License-MIT-9280FF?style=flat-square&labelColor=343B45"/></a>
 <a href="https://github.com/genesistoxical/drop-icons/releases/tag/2.1.1"><img src="https://img.shields.io/github/v/release/genesistoxical/drop-icons.svg?color=9280FF&label=Release&style=flat-square&labelColor=343B45"/></a>
 <a href="#"><img alt="NET" src="https://img.shields.io/badge/.NET_Framework-4.8-9280FF?style=flat-square&labelColor=343B45"/></a> 
 <a href="/installer%20src"><img alt="Installer" src="https://img.shields.io/badge/Installer-ISS-9280FF?style=flat-square&labelColor=343B45"/></a>
 <a href="#"><img alt="Languages" src="https://img.shields.io/badge/Idiomas-2-9280FF?style=flat-square&labelColor=343B45"/></a>
</p>

<p align="center">
<a href="README.md">English</a> :speech_balloon: <a href="README-es.md">Español</a>
</p>

## Características
* Interfaz limpia e intuitiva.
* Convertir rápidamente muchas imágenes en iconos a la vez, con la función de arrastrar y soltar.
* Cambiar entre el idioma English y Español.
* Compatibilidad con imágenes .png .jpg .jpeg .jfif .bmp .gif y .svg
* Personalizar el color del tema.
* Número de las imágenes a convertir, restando tres que se muestran como vista previa.
* Guardar los iconos en la misma carpeta (por defecto) o en una específica.
* Habilitar y deshabilitar Topmost.
* Configuración con dos opciones de formato (tamaños incluidos dentro del icono). [ⓘ](#details)
* Evitar la duplicación de una imagen que se ha añadido previamente.
* Opción para generar un icono mini.
* Esquinas adaptables (redondeadas o metro), dependiendo la versión del sistema operativo.
* Guarda la configuración en un archivo .ini, excepto para los switches.

## Previa
<a href="#"><img src="docs/assets/Drop-Icons-v2.gif"/></a>

## Uso
Arrastra y suelta tus imágenes en el espacio vacío, obtendrás una vista previa de tres imágenes excepto si solo arrastras una o dos. Más abajo puedes ver la cantidad total de imágenes a convertir, restando tres de la previa. Si no puedes arrastrar, cliquea en `Agregar`.

Deja el primer switch activado si deseas guardarlos en la misma carpeta, si prefieres elegir una carpeta específica, desactívalo. También puedes generar un icono mini activando el segundo switch. Por último, haz clic en el botón `Convertir`, espera a que la interfaz se reinicie porque eso indica que ha finalizado y tus iconos están listos.

Si necesitas eliminar las imágenes que agregaste por error, haz clic en el icono de las flechas. Recuerda que puedes arrastrar imágenes tantas veces como quieras antes de hacer clic en el botón `Convertir`.

<br id="details"/>
Dando click en el botón superior de Info, aparecerá una nueva ventana en la que puedes:

- **Cambiar el tema:** Haz clic sobre `Cambiar Tema` para abrir el selector de color y elegir uno personalizado, cuando lo tengas da clic en Aplicar. Para regresar al color por defecto repite los pasos anteriores y presiona el botón morado debajo del selector de tono, finalmente haz clic en Aplicar.

- **Cambiar el idioma:** En la sección inferior **Idioma**, haz clic en el icono de las flechitas para cambiar entre English o Español, por último da clic en el botón de regresar para aplicar y ver los cambios.
 
- **Iconos (tamaño):** Al hacer clic en `Formato` se desplegará un menú con dos opciones para elegir los tamaños que serán incluidos dentro del icono: **Múltiple** genera un icono de alta calidad que incluye todos los tamaños necesarios como 16, 32, 48, 64, 128 y 256 pixeles, aunque sus dimensiones mostrarán solo 16px. La ultima opción es **256 px** el cual genera un icono con un solo tamaño pero luce pixelado en la vista de detalles.
     >Nota: Si el switch **Generar icono mini** está activado, se creará un icono pequeño independientemente de la opción del Formato.

- **Contenido de terceros:** En la parte izquierda están los nombres de cada librería, proyecto, iconos o tipografías que fueron utilizados, cliquea uno para leer su licencia y autor(a) o autores(as), además de una corta descripción. Puedes hacer clic sobre el icono de clip para ir al repositorio/sitio oficial de cada uno y cambiar de página con **Siguiente 🢖🢖** o **🢔🢔 Atrás**.

<br>

Para elegir que Drop Icons esté encima de todas las ventanas (Topmost) o no, da clic derecho en cualquier lugar de la ventana principal y elige Habilitar Topmost o Deshabilitar Topmost.

## Opciones
<a href="#"><img src="docs/assets/Drop-Icons-Options-v2.gif"/></a>

## Instalador
Para compilar el instalador es necesario [Inno Setup](https://jrsoftware.org/isinfo.php), los archivos se encuentran en la carpeta [installer src](/installer%20src). Solo debes abrir el proyecto (Installer.iss) y compilarlo, a menos que desees hacer una modificación. Al finalizar, en la misma ubicación dejará una carpeta llamada Output.

**Portable with 7zip.bat** permite comprimir en .zip rápidamente la versión portable. Únicamente funciona con [7zip](https://www.7-zip.org/).

Ambos .iss y .bat obtienen los archivos que son necesarios dentro de su carpeta y/o la carpeta Release (debido a las rutas relativas).

## Contribuciones
* El paquete **HandyControls** dejará de actualizarse (por ahora o permanentemente) ya que la última versión no permite cambiar el tamaño de ToggleButtonSwitch.
* Si haces comentarios en el código, preferiblemente en Español, por favor.
* Los nombres de las variables deben estar en Inglés.
* Si abres un **Issue**, puede ser en Inglés o Español.
* **Pull request** en Inglés, en la descripción puedes agregar detalles en Inglés o Español.
* Al convertir **.svg** primero se convierte a **.png** en una carpeta temporal y posteriormente de **.png** a icono. La prioridad sería **.svg** "directamente" a icono.
  
## Configuración
El archivo `Config.ini` almacena información del lenguaje, color del tema, tamaño del icono y si está activada o no la opción TopMost.

~~~
[Options]
Language = en
Topmost = false

[Theme]
#FF9280FF

[Format]
Size = multiple
~~~

>Nota: las dos opciones de tipo switch no se guardan porque no son opciones que suelan activarse todo el tiempo.

## Esquinas adaptables
<a href="#"><img src="docs/assets/Drop-Icons-Corners-v2.png"/></a>

# Creditos
Drop Icons está basado en [Iconizer](https://github.com/willnode/Iconizer) bajo [MIT License](https://github.com/willnode/Iconizer/blob/master/LICENSE).

* [HandyControls](https://github.com/ghost1372/HandyControls) bajo [MIT License](https://github.com/ghost1372/HandyControls/blob/develop/LICENSE).

* [FolderBrowserEx](https://github.com/evaristocuesta/FolderBrowserEx) library bajo [MIT License](https://github.com/evaristocuesta/FolderBrowserEx/blob/master/LICENSE).

* [Noto Music](https://fonts.google.com/noto/specimen/Noto+Music) bajo [SIL Open Font License](/src/DropIcons/Docs/Noto%20Music/OFL.txt).

* Los iconos son parte de [Teenyicons](https://github.com/teenyicons/teenyicons) bajo [MIT License](https://github.com/teenyicons/teenyicons/blob/master/LICENSE).

* [SharpVectors](https://github.com/ElinamLLC/SharpVectors/) bajo [BSD 3-Clause](https://github.com/ElinamLLC/SharpVectors/blob/master/License.md).

* [WinVersion](https://github.com/shaovoon/win_version_detection) detection bajo [MIT License](https://github.com/shaovoon/win_version_detection/blob/main/LICENSE).

*Puedes encontrar todas las licencias [aquí](/src/DropIcons/Docs).*

## ¿Qué es lo nuevo?
`Versión 1.0.0` se creó en Windows Forms. Drop Icons ya no se desarrollará con esa tecnología, sin embargo, todavía puedes encontrar y/o descargar la última versión oficial aquí:
<br>
🏷️ [winforms-v1-final](https://github.com/genesistoxical/drop-icons/tree/winforms-v1-final)

<br>

`Versión 2.0.0` está desarrollada con Windows Presentation Foundation (WPF) para mejorar la interfaz e incluir esquinas redondeadas adaptables, según la versión del sistema operativo.

En este segundo lanzamiento se ha mejorado la ventana **Acerca de**, el archivo **Config.ini** se ha modificado para usar solo el color del tema HEX y no RGB, además que se ha reemplazado el selector de color (para el tema) por uno mucho más moderno.

Debido a este último cambio, se eliminó **Colors.dat** ya que no existe botón para guardar los personalizados, en su lugar hay una paleta de colores.

<br>

`Versión 2.1.1` permite convertir tres formatos más; **.jfif .gif** y **.svg**, para este último fue necesario agregar compatibilidad [📍Can you add support to SVG file?](https://github.com/genesistoxical/drop-icons/issues/2). Ahora hay opciones de tamaño para los iconos: **Múltiple** y **256 px** [📍Icon Default 256x256](https://github.com/genesistoxical/drop-icons/discussions/1).

Además de otras pequeñas mejoras, se implementó una nueva página en la ventana **Acerca de** y se agregó una carpeta con el nombre **Libs** en los binarios para una mejor organización de dll(s).

<br>

`Version 2.1.2` incluye actualizaciones menores en la ventana **Acerca de**: La configuración para los tamaños incluidos dentro del icono ahora se llama **Formato** en vez de **Iconos**, para evitar confusiones. También se actualizó un problema en un enlace de atribución, así como otros pequeños cambios en las variables del código.

## Licencia
**MIT License**

Copyright (c) 2022 - 2023 Génesis Toxical ([read here](LICENSE)).
