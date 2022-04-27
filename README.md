Reference code for the blog: [https://es.acervolima.com/creacion-de-un-backend-de-api-rest-utilizando-node-js-express-y-postgres/]

# Contruir imagen
docker build -t felipeyepes/nodejs-web:v1 .
# listar imeges
docker images
# crear un contenedor con esta imagen
-p: edita el puerto en el contenedor y lo asigna a un puerto en nuestro host. Usaremos el puerto 80 en el host, pero puede modificarlo como considere necesario si tiene otro proceso en ejecución en ese puerto. Para obtener más información sobre cómo funciona, consulte esta discusión en la documentación de Docker sobre enlaces de puerto.
-d: ejecuta el contenedor en segundo plano.
--name: permite darle al contenedor un nombre fácil de recordar.
# images
docker images -a
# Elimine el contenedor detenido y todas las imágenes, incluso las no utilizadas o pendientes, con el siguiente comando: 
docker system prune -a
# compilar y run
 docker run --name nodejs-web -p 8080:8080 -d felipeyepes/nodejs-web:v1