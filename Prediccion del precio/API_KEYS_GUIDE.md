# 🔑 Guía para Obtener API Keys Gratuitas

## 🎯 APIs Disponibles en tu App

### 1. 🟢 **Yahoo Finance** (Sin API Key - Funciona Ya)
- ✅ **Completamente gratis**
- ✅ **Sin registro requerido**
- ✅ **Datos en tiempo real**
- ⚠️ Puede tener limitaciones de CORS en algunos navegadores

### 2. 🔵 **Finnhub** (API Key Gratuita)
- 🆓 **60 llamadas por minuto gratis**
- 📊 **Datos de alta calidad**
- 🌍 **Mercados globales**

**Cómo obtener:**
1. Ve a: https://finnhub.io/register
2. Registrarse con email
3. Confirmar email
4. Ir a Dashboard → API Key
5. Copiar tu API key

### 3. 🟡 **Alpha Vantage** (API Key Gratuita)
- 🆓 **5 llamadas por minuto gratis**
- 📈 **Datos históricos incluidos**
- 🔍 **Análisis técnico**

**Cómo obtener:**
1. Ve a: https://www.alphavantage.co/support/#api-key
2. Llenar formulario simple
3. Recibir API key por email
4. Usar inmediatamente

### 4. 🟣 **Polygon.io** (API Key Gratuita Limitada)
- 🆓 **5 llamadas por minuto gratis**
- 📊 **Datos institucionales**
- 🚀 **Muy rápido**

**Cómo obtener:**
1. Ve a: https://polygon.io/signup
2. Registrarse gratis
3. Verificar email
4. Dashboard → API Keys

## 🚀 Configuración Rápida (5 minutos)

### Paso 1: Abrir tu App
```
Abre: stock-app-apis.html
```

### Paso 2: Probar Yahoo Finance (Ya funciona)
1. Busca cualquier acción (AAPL, GOOGL, etc.)
2. ¡Datos reales inmediatamente!

### Paso 3: Agregar Finnhub (Recomendado)
1. Registrarse en finnhub.io (2 minutos)
2. Copiar API key
3. En tu app: Seleccionar "Finnhub"
4. Pegar API key
5. ¡Listo!

## 📊 Comparación de APIs

| API | Gratis | Límite | Calidad | Facilidad |
|-----|--------|--------|---------|-----------|
| Yahoo Finance | ✅ | Ilimitado* | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| Finnhub | ✅ | 60/min | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| Alpha Vantage | ✅ | 5/min | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| Polygon.io | ✅ | 5/min | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ |

*Puede tener limitaciones de CORS

## 🛠️ Solución de Problemas

### Error CORS con Yahoo Finance
```javascript
// Usar proxy CORS (ya incluido en el código)
const proxyUrl = 'https://cors-anywhere.herokuapp.com/';
const targetUrl = 'https://query1.finance.yahoo.com/...';
```

### API Key Inválida
1. Verificar que copiaste la key completa
2. Revisar que no tenga espacios extra
3. Confirmar que la cuenta esté activada

### Límite de Llamadas Excedido
- **Alpha Vantage**: Esperar 1 minuto
- **Finnhub**: Cambiar a plan premium o usar otra API
- **Polygon**: Esperar o usar Yahoo Finance

## 🎯 Recomendación de Uso

### Para Uso Personal:
1. **Yahoo Finance** - Principal (gratis ilimitado)
2. **Finnhub** - Backup (60/min gratis)

### Para Desarrollo:
1. **Finnhub** - Principal (mejor calidad)
2. **Alpha Vantage** - Análisis técnico
3. **Yahoo Finance** - Backup

### Para Producción:
- Considerar planes premium
- Implementar caché de datos
- Usar múltiples APIs como fallback

## 🔧 Configuración Avanzada

### Rotar APIs Automáticamente
```javascript
const apiPriority = ['yahoo', 'finnhub', 'alpha'];
// El código ya incluye fallback automático
```

### Caché Local
```javascript
// Guardar datos por 5 minutos
localStorage.setItem(`stock_${symbol}`, JSON.stringify({
    data: stockData,
    timestamp: Date.now()
}));
```

### Proxy CORS (Si es necesario)
```javascript
// Usar servicio proxy gratuito
const proxyUrl = 'https://api.allorigins.win/raw?url=';
```

## 📈 Próximos Pasos

1. **Probar Yahoo Finance** (ya funciona)
2. **Registrarse en Finnhub** (5 minutos)
3. **Configurar Alpha Vantage** (opcional)
4. **Agregar gráficos** con Chart.js
5. **Implementar alertas** de precios

## 💡 Tips Pro

- **Combinar APIs**: Usar Yahoo para precio, Finnhub para noticias
- **Caché inteligente**: Evitar llamadas innecesarias
- **Fallback automático**: Si una API falla, usar otra
- **Monitoreo**: Trackear uso de APIs

¡Con estas APIs tendrás datos reales profesionales! 🚀