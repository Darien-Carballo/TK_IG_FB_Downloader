# Sesión de configuración inicial

## Resumen

En esta sesión se dejó preparado el entorno local del proyecto para poder ejecutar la aplicación con Python y Streamlit. La aplicación arrancó correctamente y quedó disponible en el navegador mediante `localhost:8501`.

## Lo que se configuró

- El proyecto se movió a iCloud.
- Git estaba en la rama `main`, limpia y sincronizada al inicio de la sesión.
- Se dejó intacto el Python 3.9.6 del sistema.
- Se instaló Python 3.13.15 para usarlo en este proyecto.
- Se creó el entorno virtual local con:

  ```bash
  python3.13 -m venv .venv
  ```

- Se activó el entorno virtual con:

  ```bash
  source .venv/bin/activate
  ```

- Se agregó `.venv/` al `.gitignore` de la raíz para no incluir el entorno virtual en Git.
- Se instalaron las dependencias declaradas en `requirements.txt` con:

  ```bash
  pip install -r requirements.txt
  ```

- La aplicación se inició correctamente con:

  ```bash
  streamlit run app.py
  ```

- Streamlit abrió la aplicación en Chrome mediante:

  ```text
  http://localhost:8501
  ```

## Qué significa cada comando

### `pwd`

Muestra la carpeta en la que está trabajando la terminal. Es útil para confirmar que estás dentro de `TK_IG_FB_Downloader` antes de ejecutar comandos.

### `git status`

Muestra la rama actual y si hay archivos modificados, nuevos o pendientes de guardar en Git. En esta sesión no se hizo commit ni push.

### `python --version`

Muestra qué versión de Python está usando el comando `python` en ese momento. Cuando `.venv` está activo, debe corresponder al Python del entorno virtual.

### `pip`

Es la herramienta que instala paquetes de Python. En esta sesión se usó para instalar lo que aparece en `requirements.txt` dentro de `.venv`.

### Streamlit

Streamlit es la herramienta que convierte el código Python de `app.py` en una aplicación web local. Python ejecuta la aplicación, Streamlit levanta un pequeño servidor y Chrome muestra la interfaz.

`localhost` significa “esta misma computadora” y `8501` es el puerto local donde Streamlit está escuchando.

## Qué hacer cada vez que se retome el proyecto

Desde una terminal nueva:

1. entra en la carpeta del proyecto;

   ```bash
   cd "/ruta/a/TK_IG_FB_Downloader"
   ```

2. activa el entorno virtual;

   ```bash
   source .venv/bin/activate
   ```

3. inicia la aplicación;

   ```bash
   streamlit run app.py
   ```

4. usa la dirección local que indique Streamlit, normalmente `http://localhost:8501`;
5. cuando termines, vuelve a la terminal y presiona `Control + C` para detener la app;
6. si ya no trabajarás con Python en esa terminal, puedes salir del entorno con:

   ```bash
   deactivate
   ```

No es necesario volver a crear `.venv` ni reinstalar las dependencias en cada sesión. Esos pasos solo se repiten si el entorno se elimina, se cambia de computadora o se modifican las dependencias.

## Estado al cierre de esta sesión

El proyecto quedó listo para revisión y aprendizaje de Git. Se dejaron los cambios de documentación sin commit ni push, para revisarlos antes de guardarlos en el historial.
