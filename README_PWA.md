# DropLab PWA
Esta versión es una Progressive Web App instalable desde Chrome.

## Importante
La PWA y la API están en el mismo servidor FastAPI. Por eso la app funciona al instalarla cuando el servidor está accesible.

## Ejecutar localmente
pip install -r requirements.txt
uvicorn app:app --host 0.0.0.0 --port 8000

Después abre http://IP_DEL_SERVIDOR:8000 en Chrome.

## Instalar en Pixel
Chrome → menú ⋮ → "Instalar aplicación" (o "Añadir a pantalla de inicio").

## Para usarla desde cualquier lugar
Necesita estar desplegada en un servidor HTTPS. La PWA está preparada para ello; el siguiente paso es desplegar FastAPI en un hosting compatible.
