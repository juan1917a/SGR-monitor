# Dashboard SGR — Sociedades de Garantía Recíproca (Argentina)

Dashboard interactivo para analizar y monitorear el proceso de selección
crediticia de las SGR de Argentina. Datos mensuales desde enero de 2024.

**Último dato cargado:** Septiembre 2026 · **42 SGR activas**

## Qué muestra

Archivo HTML autónomo (CSS, JS y datos embebidos; solo levanta Chart.js desde
un CDN). Filtrable por todo el sistema, por SGR individual y por rango de meses.

**Sistema:** Fondo Integrado, Garantías Vigentes, Mora Total (%), Riesgo Vivo (%),
Mora >90d (%), Apalancamiento, Liquidez (%), Inversiones en USD (%), Market Share
y ranking de SGR.

**Por SGR:** análisis en profundidad de cada SGR con su evolución en gráficos,
comparada contra el promedio del sistema.

## Definiciones

- **Fondo de Riesgo Computable** = Fondo de Riesgo (Efectivo Integrado)
- **Fondo de Riesgo Disponible** = Integrado − Mora
- **Apalancamiento** = Garantías Vigentes / Fondo de Riesgo Disponible
- **Mora Total (%)** = (Mora sin deuda proporcional / Fondo integrado) × 100
- **Riesgo Vivo (%)** = (Mora sin deuda proporcional / Garantías Vigentes) × 100
- **Mora Temprana (<90 días)** = (%_MENOR_a_31_DÍAS + %_MENOR_a_90_DÍAS)

## Fuentes

Archivos regulatorios mensuales: 01-fondos de riesgo (FDR), 02-inversiones del
FDR, 03-mora, 05-garantías vigentes.

## Publicar online (GitHub Pages)

1. Subí este repo a GitHub (el archivo del dashboard debe llamarse `index.html`).
2. Settings → Pages → Branch `main`, carpeta `/root` → Save.
3. En ~2 min queda en `https://<tu-usuario>.github.io/<repo>/`.

## Actualización mensual

Reemplazar `index.html` por la versión del mes nuevo (misma estructura; se
agregan los registros del último mes respetando solo las SGR activas al día).
