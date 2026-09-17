# Guía para mantener `README.md`

Este archivo sirve como instrucción para cualquier persona o IA que tenga que redactar o actualizar la documentación principal de `TK_IG_FB_Downloader`.

## Objetivo

Mantener un README claro, breve y verificable para una persona principiante que necesita instalar, ejecutar y entender el estado real del proyecto.

## Antes de escribir

Inspecciona primero, como mínimo:

1. `app.py` para conocer las funciones y el flujo real de la aplicación;
2. `requirements.txt` para documentar las dependencias actuales;
3. `README.md` para conservar información útil y detectar lo que quedó desactualizado;
4. `.gitignore` y la estructura de carpetas cuando cambien la configuración o la organización del proyecto.

Si existe documentación adicional relevante, úsala para entender el contexto, pero confirma las funciones en el código antes de afirmarlas como actuales.

## Cuándo actualizar el README

Actualiza `README.md` cuando cambie cualquiera de estos aspectos:

- instalación o versión mínima de Python;
- creación, activación o ubicación del entorno virtual;
- dependencias de `requirements.txt`;
- comando para ejecutar o detener la aplicación;
- estructura de archivos o carpetas;
- entradas que acepta la app;
- funciones, plataformas soportadas o resultados que produce;
- limitaciones importantes o pasos necesarios para usarla.

## Reglas de exactitud

- No inventes capacidades, integraciones, plataformas ni resultados.
- No describas una función como disponible si no está implementada y comprobada.
- Diferencia el nombre del repositorio del alcance real de la aplicación.
- Mantén los comandos alineados con los archivos existentes y con el entorno usado por el proyecto.
- Si una versión, una URL, un precio, una credencial o una configuración no está verificada, no la presentes como un hecho.
- Cuando haya una limitación, escríbela de forma directa y breve.
- Conserva información útil del README anterior, salvo que sea incorrecta o esté desactualizada.

## Organización recomendada

Mantén, cuando sea pertinente, este orden:

1. propósito del proyecto;
2. estado actual y límites;
3. requisitos;
4. instalación inicial;
5. ejecución y uso;
6. cómo detener la app;
7. estructura básica;
8. comandos útiles;
9. notas de uso responsable o limitaciones.

No agregues secciones solo para hacer el documento más largo.

## Configuración inicial frente a rutina diaria

Explica por separado:

- **Configuración inicial:** instalar Python, crear `.venv` e instalar las dependencias.
- **Rutina diaria:** entrar al proyecto, activar `.venv` y ejecutar `streamlit run app.py`.

Esto evita que una persona principiante repita pasos de instalación innecesariamente.

## Estilo

- Escribe en español claro y didáctico.
- Explica brevemente los términos técnicos cuando sea útil.
- Usa bloques de código para comandos que se puedan copiar.
- Prefiere instrucciones concretas a explicaciones abstractas.
- Mantén el README conciso: debe ayudar a usar el proyecto, no reemplazar toda la documentación técnica.
- Usa nombres y rutas exactos, respetando mayúsculas, minúsculas y espacios.

## Verificación final

Antes de guardar una actualización:

1. comprueba que cada comando mencionado corresponda al proyecto;
2. confirma que los nombres de archivos enlazados existan;
3. revisa que no se hayan prometido funciones futuras;
4. verifica que la estructura descrita coincida con las carpetas reales;
5. conserva los cambios del usuario y no hagas commit ni push salvo que se solicite expresamente.
