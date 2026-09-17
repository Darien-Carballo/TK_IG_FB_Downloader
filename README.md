# TK_IG_FB_Downloader

Es una aplicación web local, construida con Python y Streamlit, para descargar uno o varios videos de TikTok mediante `yt-dlp` y reunir las descargas exitosas en un archivo ZIP.

## Estado actual 17 de septiembre 2026 5:45 am 

El proyecto está en una etapa de prototipo.

Actualmente la app:

- acepta enlaces de TikTok, uno por línea;
- intenta descargar cada video mediante `yt-dlp`;
- muestra el avance del procesamiento;
- crea un archivo ZIP con los videos que sí se descargaron;
- permite descargar ese ZIP desde la interfaz.

El nombre del repositorio contempla TikTok, Instagram y Facebook, pero la versión actual de `app.py` solo implementa TikTok. No se deben asumir funciones para Instagram, Facebook, cuentas privadas, listas de reproducción u otros formatos hasta que aparezcan implementadas y verificadas en el código.

## Requisitos

- macOS, Windows o Linux;
- Python 3.13 instalado;
- conexión a internet para instalar las dependencias y procesar enlaces;
- una terminal;
- un navegador web.

La aplicación utiliza las dependencias declaradas en [`requirements.txt`](requirements.txt):

- `streamlit` para crear y ejecutar la interfaz web;
- `yt-dlp` para intentar obtener los videos.

## Instalación inicial

Abre una terminal y entra en la carpeta del proyecto:

```bash
cd "/ruta/a/TK_IG_FB_Downloader"
```

Comprueba que Python 3.13 esté disponible:

```bash
python3.13 --version
```

Crea el entorno virtual del proyecto:

```bash
python3.13 -m venv .venv
```

Activa el entorno virtual:

En macOS o Linux:

```bash
source .venv/bin/activate
```

En Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

Cuando esté activo, normalmente verás `(.venv)` al inicio de la línea de la terminal.

Instala las dependencias:

```bash
pip install -r requirements.txt
```

La instalación crea y utiliza un entorno aislado para este proyecto. No es necesario modificar el Python del sistema.

## Ejecutar la aplicación

Con el entorno virtual activo, inicia Streamlit:

```bash
streamlit run app.py
```

Streamlit levantará un servidor local y normalmente abrirá el navegador automáticamente. Si no lo hace, abre la dirección que muestre la terminal, normalmente:

```text
http://localhost:8501
```

Después:

1. pega uno o varios enlaces de TikTok, uno por línea;
2. pulsa **Procesar y Descargar ZIP**;
3. espera a que termine el procesamiento;
4. si hubo descargas exitosas, pulsa **Descargar archivo ZIP**.

## Detener la aplicación

Regresa a la terminal donde Streamlit está ejecutándose y presiona:

```text
Control + C
```

Esto detiene el servidor local y devuelve el control de la terminal.

## Estructura básica

```text
TK_IG_FB_Downloader/
├── app.py                 # Interfaz y lógica actual de la aplicación
├── requirements.txt       # Dependencias de Python
├── README.md              # Documentación principal
├── README_GUIDE.md        # Instrucciones para mantener este README
├── .gitignore             # Archivos excluidos de Git
└── docs/
    └── SESION_CONFIGURACION_INICIAL.md
```

## Comandos útiles

Ver la carpeta actual:

```bash
pwd
```

Revisar el estado de Git:

```bash
git status
```

Comprobar la versión de Python:

```bash
python --version
```

Comprobar la versión de `pip` dentro del entorno activo:

```bash
pip --version
```

Activar el entorno virtual en una nueva sesión:

```bash
source .venv/bin/activate
```

Actualizar las dependencias declaradas:

```bash
pip install -r requirements.txt
```

Salir del entorno virtual:

```bash
deactivate
```

## Uso responsable

La aplicación intenta descargar contenido a partir de los enlaces proporcionados. Verifica que tengas permiso para descargar y utilizar ese contenido y respeta las condiciones de uso de cada plataforma.
