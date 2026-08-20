# DropLab
App móvil/web + API local para simular productos de dropshipping.

## Ejecutar
1. Instala Python 3.11+.
2. En esta carpeta: `pip install -r requirements.txt`
3. Ejecuta: `uvicorn app:app --host 0.0.0.0 --port 8000`
4. Abre `http://TU-IP:8000` en el móvil conectado a la misma Wi‑Fi.

## API
GET /api/health
POST /api/simulate

La API acepta coste, precio, envío, comisiones, publicidad, conversión y visitas/día.
La simulación usa 5.000 escenarios Monte Carlo y devuelve beneficio medio, mediano, P10, P90 y probabilidad de beneficio positivo.

## Conexión con un análisis externo
La arquitectura deja `/api/simulate` listo para que un sistema externo envíe los productos que haya detectado y reciba las métricas. Para conectar directamente un modelo de IA necesitarás una clave de API del proveedor y un servidor público con autenticación; no se incluye ninguna clave.
