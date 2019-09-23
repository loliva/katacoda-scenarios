<pre class="file" data-filename="Dockerfile" data-target="append">RUN apk add --no-cache curl
</pre>

Dockerfile Mejores-Practicas
>El mejor uso para ENTRYPOINT es establecer el comando principal de la imagen, permitiendo que esa imagen se ejecute como si fuera ese comando (y luego usar CMD como las banderas predeterminadas).


Establecemos el punto de entrada en `curl` y establecemos` --help` como el parámetro predeterminado.

<pre class="file" data-filename="Dockerfile" data-target="append">ENTRYPOINT ["curl"]
CMD ["--help"]
</pre>

Rehacemos la imagen `docker build -t curl .`{{execute}}

Recuerda podemos ejecutar un contenedor docker con curl: `docker run --rm curl`{{execute}}


Usemos nuestro nuevo contenedor curl para recopilar información útil de la web:

`docker run --rm curl -s wttr.in/scl`{{execute}}
