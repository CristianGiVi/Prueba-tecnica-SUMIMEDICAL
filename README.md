# Guía para ejecutar Docker Compose

Este repositorio contiene un docker-compose.yml para facilitar el despliegue de la aplicación.

## Requisitos previos

- Docker instalado en tu sistema.

## Instrucciones

1. Clona este repositorio en tu máquina local

2. Ejecuta:
```bash
docker-compose up -d
```

3. Despues ejecuta el siguiente comando sustituyendo el id del docker container con el de laravel(backend):
```bash
docker exec <docker_container_id> sh -c "cd backend && php artisan migrate"
```
