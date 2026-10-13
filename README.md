El contenedor esta creado y ya en funcionamiento en el puerto 80 que he especificado en el documento Dockerfile.
sudo docker run --name web-pps -d -p 127.0.0.1:8080:8000 pps_1:latest
docker ps
curl -s -o /dev/null -w '%{http_code}\n' http://127.0.0.1:80