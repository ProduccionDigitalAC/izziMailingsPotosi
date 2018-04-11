```
   ___                   __          __               _______                       __
  / _ | ___________ ____/ /  ___ ___/ /__ _______ _  / ___/ /__ __  _____ _______  / /
 / __ |/ __/ __/ -_) __/ _ \/ -_) _  / -_) __/ _ `/ / /__/ / _ `/ |/ / -_) __/ _ \/ / 
/_/ |_/_/ /_/  \__/\__/_//_/\__/\_,_/\__/_/  \_,_/  \___/_/\_,_/|___/\__/_/  \___/_/  
                                                                                      
```
                                                                                
## Guía para Newsletters (izzi). 

El cliente utiliza Oracle y tiene bastantes restricciones a la hora de importar los Newsletters. Las siguientes recomendaciones te ayudaran a realizar tu trabajo mas facilmente. 

1. Los assets deben de estar en la raiz del html, evita guardar los assets dentro de carpetas _img_ _images_  ya que el sistema puede enviar errores por el nombre de la carpeta.

2. Si usas MacOX probablemente se llegue a filtar archivos del sistema como un .DS_store puedes apoyarte en la terminal y ejecutar **find . -name ‘*.DS_Store’ -type f -delete*** o puedes configurar tu compresor de archivos para que no incluya archivos ocultos de mac, te recomiendo utilices [Keka](http://www.kekaosx.com/es/) _Preferencias/No incluir archivos Ocultos del Sistema_. 
3. Para enviar el archivo comprimido usa el nombre de la camapaña sin mayusculas, espacios o caractereres espeiales camapanianov2021, evita nombres genericos main.zip, code.zip, master.zip, etc.
4. Los assets no deben de pasar de los _100kb c/u_ por lo que te recomiendo utilices Photoshop para la compresión de imagenes. 

Todos los puntos estan detallados por lo que no deberias de tener ningun problema a la hora de armar el newsletter.

Puedes configurar Photoshop con los siguientes ajustes a la hora de Exportar para la Web. 

Compresión JPG al 50% - ExportSlices 
Ajustes Prestablecidos - Ajustes de Salida
- Incluir Comentarios - Uncheck 
- Nombres de selector por defecto - Ninguno
- Nombre del Selector - Ninguno
- Compatibilidad de nombres de archivo - Unix

## Build
###Ajustes de Newsletter.irs
Esta Configuración sirve para exportar de PSD a HTML. 

#### Ajustes de salida Newsltter.iros
Esta configuracion sive para exportar los assets al formato del archivo y el peso maximo de los assets. 

### Default.sublime-commands & reg_replace_rules.sublime-settings
Esta configuración requiere [RegReplace](https://github.com/facelessuser/RegReplace) una extensión de Sublime Text 3 que ayudara a darle formato al HTML devuelto por Photoshop, dandole formato a las tablas y sea compatible con las mayoría los clientes de email. Corriendo pruebas en Litmus.

### tabla-responsive.sublime-snippet
Este es un snippet de Sublime Text, para usarlo posicionate antes de _<head>_ y escribe _tablacss_ y _tab_ se agregara unas lineas de CSS que volveran el newsletter responsivo.
- Tab1 = ID de la tabla 
- Tab2 = Ancho de la tabla
- Tab3 = Alto de la tabla

Tomate tu tiempo para instalar y cofigurar todos estas herramientas, si lo haces bien te ayudaran a optimizar tu trabajo.