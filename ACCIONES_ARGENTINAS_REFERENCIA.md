# 🇦🇷 Referencia de Acciones Argentinas - ADRs vs Locales

## 📊 Acciones con ADR y Local

Estas empresas tienen **dos versiones**: ADR en NYSE (USD) y Local en BYMA (ARS)

| Empresa | ADR (NYSE) | Local (BYMA) | Diferencia Ticker |
|---------|------------|--------------|-------------------|
| **Grupo Galicia** | GGAL | GGAL.BA | Mismo ticker |
| **Banco Macro** | BMA | BMA.BA | Mismo ticker |
| **Grupo Supervielle** | SUPV | SUPV.BA | Mismo ticker |
| **YPF** | YPF | YPFD.BA | ⚠️ Diferente |
| **Telecom Argentina** | TEO | TECO2.BA | ⚠️ Diferente |
| **Pampa Energía** | PAM | PAMP.BA | ⚠️ Diferente |
| **Ternium** | TX | TXAR.BA | ⚠️ Diferente |
| **Central Puerto** | CEPU | CEPU.BA | Mismo ticker |
| **Loma Negra** | LOMA | LOMA.BA | Mismo ticker |
| **Cresud** | CRESY | CRES.BA | ⚠️ Diferente |
| **Edenor** | EDN | EDN.BA | Mismo ticker |
| **IRSA** | IRSA | IRSA.BA | Mismo ticker |
| **MercadoLibre** | MELI | - | Solo ADR |
| **Globant** | GLOB | - | Solo ADR |
| **Despegar** | DESP | - | Solo ADR |

## 🔍 Casos Especiales

### YPF
- **ADR**: `YPF` (cotiza en NYSE)
- **Local**: `YPFD.BA` (cotiza en BYMA)
- **Nota**: El ticker local tiene "D" adicional

### Telecom Argentina
- **ADR**: `TEO` (cotiza en NYSE)
- **Local**: `TECO2.BA` (cotiza en BYMA)
- **Nota**: Tickers completamente diferentes

### Pampa Energía
- **ADR**: `PAM` (cotiza en NYSE)
- **Local**: `PAMP.BA` (cotiza en BYMA)
- **Nota**: El ticker local tiene "P" adicional

### Ternium
- **ADR**: `TX` (cotiza en NYSE)
- **Local**: `TXAR.BA` (cotiza en BYMA)
- **Nota**: El ticker local tiene "AR" adicional

### Cresud
- **ADR**: `CRESY` (cotiza en NYSE)
- **Local**: `CRES.BA` (cotiza en BYMA)
- **Nota**: El ADR tiene "Y" adicional

## 📈 Acciones Solo Locales (BYMA)

Estas empresas **NO tienen ADR**, solo cotizan en Buenos Aires:

- **ALUA.BA** - Aluar
- **TRAN.BA** - Transener
- **COME.BA** - Banco Comafi
- **BHIP.BA** - Banco Hipotecario
- **BYMA.BA** - Bolsas y Mercados Argentinos
- **TGSU2.BA** - Transportadora Gas del Sur
- **TGNO4.BA** - Transportadora Gas del Norte
- **BBAR** - Banco BBVA Argentina
- **VALO** - Banco de Valores
- **CGPA2** - Compañía General de Combustibles
- **MIRG** - Mirae Asset
- **ARCO** - Arcos Dorados

## 🌎 Acciones Solo ADR (NYSE)

Estas empresas argentinas **solo cotizan en NYSE**, no en BYMA:

- **MELI** - MercadoLibre
- **GLOB** - Globant
- **DESP** - Despegar.com

## 💡 Cómo Usar en la Aplicación

### Para buscar ADR (USD):
```
Escribe: GGAL
Selecciona: GGAL [NYSE-ADR]
Resultado: Precio en USD
```

### Para buscar Local (ARS):
```
Escribe: GGAL
Selecciona: GGAL [BYMA]
Resultado: Precio en ARS (usa GGAL.BA internamente)
```

## ⚠️ Notas Importantes

1. **Precios diferentes**: ADR y Local tienen precios diferentes (USD vs ARS)
2. **Horarios diferentes**: 
   - NYSE: 9:30-16:00 ET
   - BYMA: 11:00-17:00 ART
3. **Liquidez diferente**: Generalmente los ADRs tienen más liquidez
4. **Conversión**: El precio del ADR ≈ Precio Local / Tipo de Cambio

## 🔧 Para Desarrolladores

### Estructura en el código:

```javascript
// ADR
{ symbol: 'GGAL', name: 'Grupo Financiero Galicia S.A. (ADR)', market: 'USA-ADR', currency: 'USD' }

// Local
{ symbol: 'GGAL.BA', name: 'Grupo Financiero Galicia (Local)', market: 'Argentina', currency: 'ARS' }
```

### Visualización:
- **Símbolo mostrado**: Sin `.BA` (limpio)
- **Símbolo interno**: Con `.BA` (para APIs)
- **Badge**: "NYSE-ADR" o "BYMA"

---

**Última actualización**: Noviembre 2024
