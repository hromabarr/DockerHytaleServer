# 🇬🇧 Hytale Server on Docker

Ready-to-use configuration for setting up a dedicated Hytale server using Docker. Optimized for ZimaOS and CasaOS.

## 📋 Requirements

1.  Have the server files (`HytaleServer.jar` and `Assets.zip`) legally obtained via the Hytale Launcher or CLI.
2.  A Docker environment (ZimaOS, CasaOS, Ubuntu, etc.).

## 🚀 Installation

1.  Create a folder on your NAS or storage (e.g., `/DATA/hytale`).
2.  Upload your `HytaleServer.jar` and `Assets.zip` files to that folder.
3.  Import the `docker-compose.yml` file from this repository into your Docker manager.
4.  **Important:** Ensure the path in `volumes` matches your actual folder location.

## ⚙️ First Run & Authentication

The server requires manual authentication on the first run:

1.  Start the container.
2.  Open the container terminal: `sudo docker attach hytale-server`
3.  Run `/auth login device` and follow the instructions on the website.
4.  Run `/auth persistence Encrypted` to save the session permanently.
5.  **Detach** from the console using `Ctrl+P` followed by `Ctrl+Q` (Do not use Ctrl+C).

## 🌐 Ports

Open port **5520 UDP** (or TCP/UDP) on your router.

## 🎮 Enjoy

* **Local connection:** Use your local IP (e.g., `192.168.1.XX:5520`).
* **External connection:** Use your Public IP (check whatismyip.com) followed by the port `:5520`.

---
---

# 🇪🇸 Servidor de Hytale en Docker

Configuración lista para usar para montar un servidor dedicado de Hytale utilizando Docker. Optimizada para ZimaOS y CasaOS.

## 📋 Requisitos

1.  Tener los archivos del servidor (`HytaleServer.jar` y `Assets.zip`) obtenidos legalmente desde el Hytale Launcher o CLI.
2.  Un entorno con Docker.

## 🚀 Instalación

1.  Crea una carpeta en tu NAS o BD (ej: `/DATA/hytale`).
2.  Sube tus archivos `HytaleServer.jar` y `Assets.zip` a esa carpeta.
3.  Importa el archivo `docker-compose.yml` de este repositorio en tu gestor de Docker.
4.  **Importante:** Asegúrate de que la ruta en `volumes` coincida con tu carpeta real.

## ⚙️ Primer inicio y Autenticación

El servidor requiere autenticación manual la primera vez:

1.  Inicia el contenedor.
2.  Abre la terminal del contenedor: `sudo docker attach hytale-server`
3.  Ejecuta `/auth login device` y sigue las instrucciones de la web.
4.  Ejecuta `/auth persistence Encrypted` para guardar la sesión permanentemente.
5.  **Sal de la consola** usando `Ctrl+P` seguido de `Ctrl+Q` (No uses Ctrl+C).

## 🌐 Puertos

Abre el puerto **5520 UDP** (o TCP/UDP) en tu router.

## 🎮 Disfruta

* **En local:** Coloca la IP local (ej: `192.168.1.XX:5520`).
* **Fuera de la red:** IP Pública (cualesmiip.com) seguida del puerto `:5520`.
