---
title: 'Documentación '
---

 
 
 
 
![](images%20%282%29.jpg)

**Estructura de carpetas PHP GRAV**



Grav tiene estrucuturas de php que son de mucha importancia donde profundizaremos cada una de ellas y al final indicare si son de importancia o no

**1. **  ** / assets**
Es utilizada para almacenar archivos procesados como cssy  y jsarchivos.

**2. **  ** /backup**
Es una carpeta donde tiene almacenado la ubicación predeterminada para copias de seguridad Grav.

**3. **  ** / bin**
See la utiliza para realizar algunas tareas prácticas desde la línea de comandos, es relativamente destinada principalmente para los desarrolladores

**4. **  ** /cache**
Se usa para almacenar archivos en caché temporales que Grav genera automáticamente para mejorar el rendimiento. 

**5. **  ** / images**
Grav contiene una biblioteca de manipulación de imágenes potente pero muy fácil de usar por lo cual esta carperta almacenan images para que puedan reutilizarse si se solicita nuevamente la misma imagen con el mismo tamaño y los genera automáticamente.

**6. **  ** /logs**
Cuando Grav detecta algun error, o si tiene activado el registro o la creación de perfiles adicionales,  esta carpeta almacena los archivos de registro relevantes.

**7. **  ** / system**
Esta carpeta es muy importante y no ahi que tocarla ya que esta se encarga de que tu GRAV funcione de manera correcta  donde se  realiza diversas configuraciones que están separadas en varias secciones y cada una de estas cumple una funcion en GRAV.

* ** / src : ** Son las que contiene las independecias de GRAV. 
*  ** / assets : ** Permite configurar las opciones relacionadas con el Administrador de Activos (JS, CSS). 
* ** / blueprints : ** Determinan cómo aparecen los complementos y temas en el back-end del sitios, se configura o bien usando dentro del GRAV como                                                                 administrador o  tambien dentro del tema o el archivo principal YAML del complemento./config.
* ** /images : ** Permite configurar las  capacidades de registro alternativas para Grav CMS.
* ** /lenguajes : ** Establece la configuración de idioma del sitio y que sean compatibles,  la designación del idioma predeterminado en las URL y las traducciones.
* ** /templates : ** Aquí es donde se guardan todos los templates que se descargan y podras configurar desde aqui.
* ** /pages : ** Aquí es donde se guardan todos los templates que se descargan y podras configurar desde aqui.
* ** install.php: ** El es encargado de  las instalaciones que se hacen dentro del CMS.  

**8. **  ** /user**
Esta es una de las carpetas más importante para la mayoría de usuarios en Grav es donde porque almacena y utiliaz complementos y editando sus temas. 

* ** /user/accounts : ** Aqui se definirá las cuentas de usuario si se requieren restricciones de acceso a ciertas partes de su sitio.
* ** /user/blueprints : ** Blueprintscarpeta contiene sus planos personalizados para el sitio y de cada usuario.
* ** /user/config : ** Se utilizan para configurar el sitio web y que hayan analizado los archivos de configuracion.
* ** /pages : ** Aquí es donde se guardan todos los templates que se descargan y podras configurar desde aqui.
* ** /user/data ** GRAV utiliza la carpeta para almacenar datos como por ejemplo los Formularios que puede tomar un formulario web y almacenar los datos enviados en un                             archivo de texto en esta carpeta.
* ** /user/images: ** Se utiliza para almacenar sus imágenes y para acceder a esta carpeta se escribe  image://stream.
* ** /user/languages: ** Contiene las anulaciones de traducción que son aquellas que permite al CMS traducir el idioma a otro.
* ** /user/pages: ** Este es el corazón de Grav donde puedes crear y editar tu sitio web.
* ** /user/plugins: ** Es un complemento donde puede extender el núcleo rápido de Grav con las características particulares que puede necesitar para su sitio web.
* ** /user/themes: ** Un tema convierte tu contenido en un verdadero sitio web. 


**9. **  ** / vendo**
Es una carpeta donde contiene bibliotecas importantes en las que se basa Grav y no podemos editarla.

**10. **  ** /webserver-configs**
Es una carpeta que contiene las configuraciones de servicios web que  incluyen los valores predeterminados necesarios para Grav.

**12. **  ** Defines.php**
El es encargado de definir todas las extensiones y los tipos de contenidos de GRAV.

**13. **  ** index.php**
Es el que contienen la información de inicio del sitio web.

**14. **  ** robots**
Contiene la configuración para que los buscadores puedan encontrar el sitio de una forma rápida.

**14. **  **.htacces**
Es algo del servidor según el que estés usando puede tener configuración para apache o nginx.

**14. **  ** Licenses**
Es la licencia del CMS por lo general debe estar que es opensuse.


**14. **  ** Composer.json y Composer.lock**
Son archivos de dependencia del mismo composer


Todas estas carpetas y subcarpetas que tienen Grav son necesesarias porque permiten que tu sitio web funcione de manera correcta y asi podras configurar y realizar  cambios y  todo lo que tu le hagas a tu cms se almacenaran dentro de ellas ya que cada una de estas carpetas tienen un proposito en GRAV.



