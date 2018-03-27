update# izziMailingsPotosi

## Este un archivo de ayuda para el proximo Frontend en la Agencia. 

El cliente utiliza Oracle y tiene bastantes restricciones a la hora de importar los Newsletters. 
por lo que las siguientes recomendaciones te serviran para evitar dolores de cabeza y repetir el trabajo varias veces. Ya me lo agadreceras =) 

1. Los assets deben de estar dentro de una carpeta llamada **img/** no deben de contenter espacios ni signos. 
2. Si usas Mac probablemente se llegue a filtar un .DS_store puedes apoyarte en la terminal y ejecutar **find . -name ‘*.DS_Store’ -type f -delete** o puedes configurar tu compresor de archivos para que no incluya archivos ocultos de mac, te recomiendo utilices [Keka](http://www.kekaosx.com/es/)
3. Para enviar el arvhivo comprimido usa el nombre de la camapaña sin mayusculas, espacios o caractereres especiales camapaniaNov2021, evita nombres genericos main.zip, code.zip, master.zip, etc.
4. Los assets no deben de pasar de los 100kb c/u por lo que te recomiendo utilices Photoshop para la compresión de imagenes. 

Todos los puntos estan detallados por lo que no deberias de tener ningun problema a la hora de enviar tus archivos.

Pero como todo puede pasar puedes configurar Photoshop con los siguientes ajustes a la hora de Exportar para la Web. 

Compresión JPG al 50% - ExportSlices 
Ajustes Prestablecidos - Ajustes de Salida
- Incluir Comentarios - Uncheck 
- Nombres de selector por defecto - Ninguno
- Nombre del Selector - Ninguno
- Compatibilidad de nombres de archivo - Unix
- Colocar imagebes en la carpeta - img 
