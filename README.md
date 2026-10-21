# Deriv Tick Analyzer

Aplicación web de un solo archivo (`index.html`) para análisis estadístico en tiempo real
del **último dígito** de los ticks de índices sintéticos de volatilidad de Deriv.

- ✅ Conexión pública WebSocket: `wss://ws.derivws.com/websockets/v3?app_id=1089` (métodos `ticks_history` + `ticks`)
- ✅ Cola FIFO de capacidad configurable (por defecto 300 ticks)
- ✅ Frecuencia absoluta y relativa (%) por dígito 0–9, barras visuales y gráfico canvas
- ✅ Reconexión automática con backoff exponencial + heartbeat `ping` cada 30 s
- ✅ Controles Iniciar / Pausar / Reiniciar, indicador de estado, sin autenticación ni trading

## Uso
Abre `index.html` directamente en el navegador, o sírvelo localmente:

```bash
python3 -m http.server 8000   # → http://localhost:8000
```
