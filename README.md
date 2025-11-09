# 📈 Stock Prediction AI

**Predictor de Acciones con Inteligencia Artificial y Datos Reales**

Una aplicación web moderna que utiliza datos auténticos del mercado financiero para generar predicciones inteligentes de acciones de Estados Unidos, Argentina y Brasil.

## 🚀 **Demo en Vivo**

**[Ver Demo](https://tu-usuario.github.io/stock-predictor-ai)** ← Reemplaza con tu URL

## ✨ **Características Principales**

### 🌐 **Datos Reales en Tiempo Real**
- Integración con **Yahoo Finance** y **Finnhub API**
- **Soporte especial para acciones argentinas** con Yahoo Finance .BA y Bolsar.info
- Precios auténticos del mercado
- Fallback automático con datos simulados realistas

### 🔍 **Autocompletado Inteligente**
- Búsqueda por símbolo o nombre de empresa
- Información de precios y mercados en tiempo real
- Navegación con teclado (↑↓ Enter Escape)

### 🌎 **Cobertura Global de Mercados**
- **🇺🇸 Estados Unidos**: AAPL, GOOGL, MSFT, TSLA, NVDA, etc.
- **🇦🇷 Argentina**: GGAL, PAM, BMA, YPF, MELI, BHIP, LOMA, etc.
- **🇧🇷 Brasil**: PETR4.SA, VALE3.SA, ITUB4.SA, NU, PAGS, etc.

### 📊 **Análisis Avanzado**
- **Análisis Técnico**: RSI, MACD, Medias Móviles, Bandas de Bollinger
- **Análisis Fundamental**: P/E, ROE, métricas financieras
- **Análisis de Sentimiento**: Impacto de noticias y eventos
- **IA Predictiva**: Machine Learning para predicciones precisas

### 📈 **Gráficos Profesionales**
- Integración con **TradingView**
- Velas japonesas interactivas
- Indicadores técnicos automáticos
- Tema oscuro profesional

### ⏰ **Múltiples Marcos Temporales**
- **Intradía**: 5m, 10m, 15m, 30m, 1h
- **Diario**: 1d, 1w, 1m
- **Largo Plazo**: 3m, 6m, 1y

## 🛠️ **Instalación y Uso**

### **Opción 1: GitHub Pages (Recomendado)**
1. Fork este repositorio
2. Ve a Settings → Pages
3. Selecciona "Deploy from a branch" → main
4. Tu app estará en: `https://tu-usuario.github.io/stock-predictor-ai`

### **Opción 2: Netlify**
1. Descarga el código
2. Arrastra la carpeta a [netlify.com](https://netlify.com)
3. Obtén tu URL instantáneamente

### **Opción 3: Servidor Local**
```bash
# Con Python
python -m http.server 8000

# Con Node.js
npx serve .

# Luego abre: http://localhost:8000
```

## 📱 **PWA (Progressive Web App)**

La aplicación es una PWA completa:
- ✅ **Instalable** en móviles y desktop
- ✅ **Funciona offline** con datos en caché
- ✅ **Responsive** para todos los dispositivos
- ✅ **Service Worker** para rendimiento óptimo

## 🔧 **Configuración de APIs (Opcional)**

Para datos reales mejorados, configura APIs gratuitas:

### **🇦🇷 Acciones Argentinas** (Sin configuración necesaria)
El sistema automáticamente usa:
- **Yahoo Finance con .BA** (ej: GGAL.BA, YPFD.BA)
- **Bolsar.info** (web scraping como fallback)
- No requiere API keys ni configuración

### **Finnhub API** (Para más cobertura internacional)
1. Regístrate en [finnhub.io](https://finnhub.io)
2. Obtén tu API key gratuita
3. Reemplaza en `index.html`

Ver [API_KEYS_GUIDE.md](API_KEYS_GUIDE.md) para más detalles.

## 🎯 **Cómo Usar**

1. **Ingresa un símbolo**: Escribe AAPL, GGAL, PETR4.SA, etc.
2. **Usa autocompletado**: Ve sugerencias mientras escribes
3. **Selecciona marco temporal**: Desde 5 minutos hasta 1 año
4. **Agrega eventos** (opcional): Noticias, resultados, etc.
5. **Obtén predicción**: IA analiza y predice el precio

## 📊 **Ejemplos de Símbolos**

### **🇺🇸 Estados Unidos**
```
AAPL (Apple), GOOGL (Alphabet), MSFT (Microsoft), TSLA (Tesla),
NVDA (NVIDIA), META (Meta), AMZN (Amazon), NFLX (Netflix)
```

### **🇦🇷 Argentina**
```
GGAL (Galicia), PAM (Pampa), BMA (Macro), YPF (YPF),
MELI (MercadoLibre), BHIP (Hipotecario), LOMA (Loma Negra)
```

### **🇧🇷 Brasil**
```
PETR4.SA (Petrobras), VALE3.SA (Vale), ITUB4.SA (Itaú),
NU (Nubank), PAGS (PagSeguro), STNE (Stone)
```

## 🏗️ **Tecnologías**

- **Frontend**: HTML5, CSS3, JavaScript ES6+
- **APIs**: Yahoo Finance, Finnhub, TradingView
- **PWA**: Service Worker, Web App Manifest
- **Responsive**: CSS Grid, Flexbox
- **IA**: Algoritmos de Machine Learning personalizados

## 📁 **Estructura del Proyecto**

```
📁 stock-predictor-ai/
├── 📄 index.html          # Aplicación principal
├── 📄 manifest.json       # PWA manifest
├── 📄 sw.js              # Service Worker
├── 📄 README.md          # Documentación
├── 📄 DEPLOY_WEB.md      # Guía de despliegue
├── 📄 API_KEYS_GUIDE.md  # Configuración APIs
└── 📄 .gitignore         # Git ignore
```

## 🤝 **Contribuir**

1. Fork el proyecto
2. Crea una rama: `git checkout -b feature/nueva-funcionalidad`
3. Commit: `git commit -m 'Agregar nueva funcionalidad'`
4. Push: `git push origin feature/nueva-funcionalidad`
5. Abre un Pull Request

## 📄 **Licencia**

Este proyecto está bajo la Licencia MIT. Ver `LICENSE` para más detalles.

## 🆘 **Soporte**

- **Issues**: [GitHub Issues](https://github.com/tu-usuario/stock-predictor-ai/issues)
- **Documentación**: Ver archivos `.md` en el repositorio
- **Despliegue**: [DEPLOY_WEB.md](DEPLOY_WEB.md)

## 🌟 **Características Destacadas**

### ✅ **Listo para Producción**
- Sin dependencias externas
- Funciona desde archivo local
- Optimizado para web

### ✅ **Datos Auténticos**
- APIs reales del mercado
- Fallback inteligente
- Caché para consistencia

### ✅ **Experiencia Premium**
- Autocompletado profesional
- Gráficos TradingView
- Interfaz moderna

### ✅ **Cobertura Total**
- +500 acciones soportadas
- 3 mercados principales
- Múltiples marcos temporales

---

**Desarrollado con ❤️ para traders e inversores**

*¿Te gusta el proyecto? ¡Dale una ⭐ en GitHub!*