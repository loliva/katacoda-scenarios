FROM (Dockerfile Mejores-Practicas)

>Siempre que sea posible, use los repositorios oficiales actuales como base para sus imágenes.
Recomendamos la imagen Alpine ya que está estrechamente controlada y es de tamaño pequeño (actualmente menos de 5 MB),
mientras sigue siendo una distribución completa de Linux.

LABEL (Dockerfile Mejores-Practicas)
>Puede agregar etiquetas a su imagen para ayudar a organizar las imágenes por proyecto, registrar la información de licencia, para ayudar en la automatización o por otros motivos. Para cada etiqueta, agregue una línea que comience con LABEL y con uno o más pares clave-valor. Los siguientes ejemplos muestran los diferentes formatos aceptables.


<pre class="file" data-filename="Dockerfile" data-target="replace">FROM alpine:3.8
LABEL maintainer="Taller Docker"
LABEL organization="Coredevx"
</pre>

Reconstruye la imagen `docker build -t curl .`{{execute}}.

Ahora debería funcionar. La nueva imagen de curl docker ahora debería ser parte de nuestras imágenes locales de docker. Vamos a verlo:

`docker image inspect curl`{{execute}}          

`docker image`{{execute}} 
