# ⏱️ Segmentación de la Ineficiencia de Momentum

Latencia RSI vs SMA por País y Sector

## 📌Descripción del proyecto

Este proyecto identifica ineficiencias estructurales del mercado midiendo la latencia temporal entre:
- una señal temprana de debilidad de momentum (RSI < 50)
- y su confirmación tardía por debilidad de tendencia (Precio < SMA 50)
- El análisis se segmenta por sector y país de cotización, revelando qué combinaciones reaccionan más lentamente a la información.

## 🧠Insight financiero

- ¿En qué sectores y países el mercado tarda más en confirmar una señal de debilidad, indicando menor eficiencia informacional?

Si el RSI avisa primero pero el precio tarda días en romper la SMA:

- el mercado procesa lento la información
- existen ventanas de ventaja táctica
- se evidencia fricción, baja liquidez o sesgo conductual

## 💼Valor de negocio

🧭 Mapa de ineficiencia por geografía y sector

📉 Optimiza timing de entradas/salidas

🤖 Ideal para estrategias cuantitativas de anticipación

🌍 Aplica a rotación internacional de capital

Este insight es clave para:
- trading sistemático
- selección de mercados “lentos”
- arbitraje estadístico

## 🗄️Tablas utilizadas

- indicadores_tecnicos
- RSI 14, SMA 50, fechas
- precios_diarios
- Precio de cierre
- tickers
- Sector y país / bolsa de cotización

## ⚙️Metodología

1️⃣ Construcción de señales técnicas

Para cada ticker y fecha:

Señal RSI débil → RSI < 50

Señal SMA débil → Close < SMA 50

2️⃣ Detección de cruces

Se identifican:

📅 Fecha exacta donde RSI cruza a debilidad

📅 Fecha exacta donde SMA confirma la debilidad

Solo se consideran activaciones reales (0 → 1).

3️⃣ Cálculo de latencia

Se calcula:

Latencia = Fecha cruce SMA – Fecha cruce RSI


Esto mide cuántos días tarda el mercado en confirmar lo que el momentum ya anticipó.

4️⃣ Agregación estructural

Los resultados se agrupan por:
- Sector
- País / Bolsa
- Se exige un mínimo de 5 tickers para robustez estadística.

## 📊Interpretación de resultados

Latencia baja (0–2 días)
→ Mercado eficiente, rápida absorción de información

Latencia media (3–6 días)
→ Ineficiencia moderada, oportunidades tácticas

Latencia alta (> 7 días)
🔥 Mercado lento
💡 Alta ventaja para señales adelantadas
⚠️ Riesgo de sobre-reacción tardía

## 🚀Posibles extensiones

- Separar latencia alcista vs bajista
- Incorporar volumen como confirmación
- Medir performance real post-señal
- Crear un ranking de mercados ineficientes
- Usar como input para modelos de ejecución

## 🧩Conclusión

- Este proyecto no busca señales…
- Busca dónde las señales funcionan mejor.
- Al cruzar momentum, tendencia, sector y país, se construye un mapa cuantitativo de eficiencia de mercado, extremadamente valioso para estrategias avanzadas.
- Es análisis técnico, pero con inteligencia estructural.

## 👤Autora
Flavia Hepp Proyecto de SQL aplicó un análisis de riesgo basado en eventos.
