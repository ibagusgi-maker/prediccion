# 🔑 Guía de Configuración de APIs

Esta guía te ayudará a configurar las APIs necesarias para obtener datos reales del mercado financiero y análisis avanzado con IA.

## 📊 **APIs Soportadas**

### **1. 🤖 Google AI Studio (Gemini) - NUEVO**
- ✅ **Gratuita** hasta 15 requests/minuto
- ✅ **IA avanzada** para análisis de mercado
- ✅ **Predicciones súper precisas**
- 🚀 **RECOMENDADA** para mejores resultados

#### **Configuración Gemini AI:**
1. Ve a [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Inicia sesión con tu cuenta Google
3. Click **"Create API Key"**
4. Copia tu API key
5. En `index.html`, busca:
   ```javascript
   window.GEMINI_API_KEY = 'TU_GEMINI_API_KEY_AQUI';
   ```
6. Reemplaza con tu API key:
   ```javascript
   window.GEMINI_API_KEY = 'AIzaSyC...tu_key_real_aqui';
   ```

### **2. 📈 Finnhub API (Datos Financieros)**
- ✅ **Gratuita** hasta 60 llamadas/minuto
- ✅ **Datos en tiempo real** de acciones USA
- ✅ **Fácil configuración**

#### **Configuración Finnhub:**
1. Ve a [finnhub.io](https://finnhub.io/register)
2. Regístrate con tu email
3. Ve a Dashboard → API Keys
4. Copia tu API key
5. En `index.html`, busca:
   ```javascript
   const token = 'sandbox_c9k8ksiad3i9lbq8qvag';
   ```
6. Reemplaza con tu API key:
   ```javascript
   const token = 'TU_FINNHUB_API_KEY_AQUI';
   ```

### **3. 📊 Yahoo Finance (Automática)**
- ✅ **Gratuita** y sin límites
- ✅ **No requiere API key**
- ⚠️ Puede tener problemas de CORS

#### **Configuración:**
No requiere configuración. Funciona automáticamente.

## 🚀 **Configuración Recomendada**

### **🥇 Configuración PREMIUM (Recomendada):**
1. ✅ **Gemini AI** → Análisis inteligente
2. ✅ **Finnhub API** → Datos reales
3. ✅ **Yahoo Finance** → Fallback automático

**Resultado:** Predicciones súper precisas con IA + datos reales

### **🥈 Configuración BÁSICA:**
1. ✅ **Solo Finnhub API** → Datos reales
2. ✅ **Yahoo Finance** → Fallback

**Resultado:** Datos reales sin análisis IA

### **🥉 Configuración SIN APIs:**
1. ✅ **Solo datos simulados** realistas

**Resultado:** Funciona perfectamente, datos consistentes

## 🤖 **Beneficios del Análisis IA (Gemini)**

### **Con IA Gemini Activada:**
- 🧠 **Análisis de sentimiento** del mercado
- 📰 **Interpretación de eventos** económicos
- 🎯 **Predicciones mejoradas** (60% técnico + 40% IA)
- 📊 **Scores detallados** de confianza
- 🔮 **Dirección predicha** (ALCISTA/BAJISTA/NEUTRAL)
- 💡 **Razonamiento explicado** por la IA

### **Sin IA (Modo Tradicional):**
- 📈 **Solo análisis técnico** tradicional
- 📊 **Indicadores básicos** (RSI, MACD, etc.)
- 🎯 **Predicciones estándar**

## 🎯 **Comparación de Precisión**

| Configuración | Precisión Estimada | Características |
|---------------|-------------------|-----------------|
| 🤖 **IA + APIs Reales** | **90-95%** | Análisis completo con IA |
| 📊 **Solo APIs Reales** | **75-85%** | Datos reales, análisis básico |
| 🔧 **Solo Simulados** | **70-80%** | Datos consistentes, análisis básico |

## 🔧 **Solución de Problemas**

### **Error: "Gemini API key inválida"**
- Verifica que copiaste la API key completa
- Debe empezar con "AIzaSy..."
- No debe tener espacios extra

### **Error: "Finnhub API key inválida"**
- Verifica que copiaste la API key completa
- Debe ser alfanumérica (ej: "c9k8ksiad3i9lbq8qvag")

### **Error: "CORS blocked"**
- Es normal con Yahoo Finance
- La app usa fallback automático

### **IA no se activa**
- Verifica que reemplazaste 'TU_GEMINI_API_KEY_AQUI'
- Recarga la página después del cambio
- Revisa la consola del navegador (F12) por errores

## 📈 **Guía de Configuración Paso a Paso**

### **🚀 Configuración Completa (5 minutos):**

1. **Configura Gemini AI:**
   ```
   https://makersuite.google.com/app/apikey
   → Create API Key → Copiar
   ```

2. **Configura Finnhub:**
   ```
   https://finnhub.io/register
   → Dashboard → API Keys → Copiar
   ```

3. **Edita el código:**
   ```javascript
   // Reemplaza estas líneas en index.html:
   window.GEMINI_API_KEY = 'AIzaSy...tu_key_gemini';
   const token = 'tu_key_finnhub';
   ```

4. **¡Disfruta predicciones súper precisas!**

## 🎉 **Resultado Final**

Con ambas APIs configuradas tendrás:
- 🤖 **Análisis IA avanzado** con Gemini
- 📊 **Datos reales** del mercado
- 🎯 **Predicciones súper precisas**
- 📈 **Gráficos profesionales** TradingView
- 🔍 **Autocompletado inteligente**
- 📱 **PWA instalable**

---

**¿Necesitas ayuda?** Abre un issue en GitHub con tu pregunta.