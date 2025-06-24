# 💊PP IV Proyecto "Sistema Inteligente de Control de Stock para Farmacias" — Despliegue con Docker y Docker Hub

## Integrantes:
- Garriga, Ezequiel
- Maciel, Fernando
- Sivila, Gabriel

---

Este repositorio contiene los archivos necesarios para desplegar la aplicación Stock Farmacia usando imágenes ya publicadas en Docker Hub.

---

## 🐳 Requisitos

- Tener instalado Docker
- Tener instalado Docker Compose

---

## 🚀 Cómo levantar la aplicación

1. Cloná este repositorio:

```bash
git clone https://github.com/fercuche/app-stock-farmacia-dockerhub.git
cd app-stock-farmacia-dockerhub
```
2. Copiá el archivo de ejemplo de variables de entorno para crear el archivo .env:

```bash
cp .env.example .env
```
3. Editá el archivo .env para ajustar las variables si es necesario.
4. Construcción y despliegue de los contenedores:

```bash
docker-compose up -d
```

5. Verificá que los contenedores estén corriendo correctamente:

```bash
docker ps
```
Deberías ver los contenedores:

- farmacia_postgres
- farmacia_backend
- farmacia_frontend
  
## 🌐 Acceso a la Aplicación

Una vez que todos los servicios estén corriendo:

- **Frontend**: http://localhost
  - Usuario administrador: admin@farmacia.com / Admin123!
- **Backend API**: http://localhost:3000
- **Documentación API**: http://localhost:3000/api-docs
- **Estado del servidor**: http://localhost:3000/api/status
