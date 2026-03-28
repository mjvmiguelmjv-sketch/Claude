---
name: thumbnail
description: Genera miniaturas de máximo CTR para YouTube, Instagram, Pinterest y otras plataformas. Investiga diseño visual extremo y psicología del click, construye brief detallado, y LO GENERA DIRECTAMENTE EN CANVA. Nivel diseño gráfico profesional + máxima viralidad. Úsalo cuando el usuario quiera crear una miniatura, thumbnail, portada o imagen de preview.
---

# Skill: /thumbnail — Sistema de Miniaturas de Máximo CTR

## Cómo invocar
```
/thumbnail [plataforma] [tema/título del contenido] [condiciones opcionales]
```
Condiciones opcionales: sin cara, con cara, estilo, colores, texto específico, emoción objetivo.
Si falta contexto esencial → pregunta: plataforma, tema exacto, audiencia.

---

## PROCESO COMPLETO — ORDEN ESTRICTO, SIN SALTARSE NINGUNA FASE

---

### FASE 1A: INVESTIGACIÓN DE PATRONES VISUALES DEL NICHO

Ejecuta estas 3 búsquedas con `WebSearch`:
1. `"[tema] YouTube thumbnail best CTR 2025 design examples"`
2. `"[nicho] thumbnail color psychology high click-through viral"`
3. `"[tema] thumbnail design breakdown what works [plataforma]"`

**Extrae y documenta:**

**COLORES Y CONTRASTE:**
- Combinaciones dominantes en top thumbnails del nicho
- ¿Warm tones (rojo, naranja, amarillo) o cool tones (azul, verde, púrpura)?
- YouTube tiene interfaz blanco/gris → thumbnails que más destacan usan colores saturados
- Combinaciones de alto CTR probadas: Rojo/Amarillo, Azul/Naranja, Negro/Verde Lima, Púrpura/Dorado
- Test de escala de grises: si sin color no hay contraste, falla en pantallas con bajo brillo

**TIPOGRAFÍA EN THUMBNAIL:**
- ¿Hay texto? (regla: máx 3-5 palabras — es un hook, no un resumen)
- Estilo: bold condensed, impact, display, serif dramático
- Posición: zona superior o central (NUNCA zona inferior derecha = timestamp YouTube)
- Power words dominantes del nicho: "secreto", "nunca", "finalmente", "error", "esto cambia todo", números grandes

**COMPOSICIÓN Y PSICOLOGÍA:**
- ¿Cara humana? (thumbnails con cara emocional: +25-30% CTR según A/B tests 2025)
- Expresión facial: genuina y relatable supera a la exagerada "YouTube face" en 73% de casos
- Mirada directa a cámara = conexión; mirada hacia elemento = dirige atención del espectador
- Regla de los 2 focos máximos: sujeto principal + texto/elemento secundario. Más = clutter
- Curiosity gap: mostrar el "qué" pero ocultar el "cómo" → +50% CTR potencial
- Efecto Zeigarnik: acción en progreso > resultado final (el cerebro necesita cerrar el loop)
- Juxtaposición: contrastes visuales/conceptuales que crean tensión cognitiva

**BENCHMARKS TÉCNICOS:**
- Tiempo de decisión del espectador: 1.8 segundos
- Contraste ratio mínimo para móvil: 4.5:1
- 69% del tráfico YouTube es móvil → elementos grandes, sin texto diminuto
- Thumbnails con cara reciben hasta 921.000 vistas más de media (2025)

---

### FASE 1B: ANÁLISIS DE COMPETENCIA DEL NICHO

Ejecuta con `WebSearch`:
1. `"top [nicho] YouTubers thumbnail style what makes them work"`
2. `"[nicho] YouTube thumbnail A/B test winner 2025"`

Extrae: qué diferencia visualmente los thumbnails de alto CTR de los de bajo CTR en este nicho específico. Busca el patrón que se repite en los top 10.

---

### FASE 1C: PRESENTACIÓN DE INVESTIGACIÓN

```
## Investigación: thumbnail [plataforma] para "[tema]"

SISTEMA DE COLOR RECOMENDADO:
- Fondo: [hex/descripción] — justificación basada en datos
- Elemento principal: [hex/descripción]
- Texto: [hex] + contraste estimado [X]:1
- Combinación de contraste: [par de colores recomendado]

TIPOGRAFÍA:
- Estilo: [descripción específica]
- Texto propuesto: "[máx 5 palabras]"
- Power word: [palabra + por qué funciona en este nicho]
- Posición: [zona exacta del thumbnail]

COMPOSICIÓN:
- Elemento principal: [descripción visual]
- ¿Cara? [sí/no + expresión si aplica]
- Focos de atención: [descripción — máx 2]
- Técnica psicológica: [curiosity gap / Zeigarnik / juxtaposición / emoción]

PATRONES DEL NICHO:
[2-3 patrones específicos identificados en thumbnails de alto rendimiento]

ESTRATEGIA:
[2 frases: combinación visual+psicología que ganará en este nicho específico]
```

---

### FASE 2: BRIEF DE 3 VARIACIONES

Genera siempre 3 conceptos con enfoques distintos:

```
VARIACIÓN A — [nombre concepto]
Enfoque: [descripción del ángulo visual]
Texto overlay: "[texto exacto]"
Elemento principal: [descripción visual dominante]
Técnica psicológica: [la que usa]
Emoción objetivo: [qué siente el espectador]

VARIACIÓN B — [nombre concepto]
[...]

VARIACIÓN C — [nombre concepto]
[...]
```

Pregunta al usuario si quiere ajustar alguna variación antes de generar.

---

### FASE 3: GENERACIÓN EN CANVA — OBLIGATORIA, SIEMPRE

Usa `generate-design` para cada variación. Query ultra-detallado con hex codes, tipografía específica, copy exacto y descripción de composición.

**Estructura del query para máximo resultado:**
```
[Plataforma] thumbnail for "[tema exacto del contenido]".

MAIN VISUAL: [descripción detallada del elemento principal — sujeto, objeto, escena].
FACE/EXPRESSION: [si aplica — expresión específica relatable, direct eye contact / looking at element].
BACKGROUND: [hex color o descripción] — high saturation to stand out against YouTube's white/gray interface.
COLOR SYSTEM: [color principal hex], [color acento hex], [color texto hex]. Contrast ratio 4.5:1 minimum.
TEXT OVERLAY: "[texto exacto — máx 5 palabras]" positioned in [upper third / center / left side].
TYPOGRAPHY: Bold condensed [sans-serif/display/impact style], [color del texto], large and highly legible at small sizes.
COMPOSITION: [rule of thirds / centered / asymmetric]. Maximum 2 focal points.
PSYCHOLOGY: [curiosity gap showing X but hiding Y / Zeigarnik effect: action in progress / visual juxtaposition of A and B].
STYLE: [hyperrealistic photo / graphic design / photo+text overlay / illustration + text].
MOBILE OPTIMIZATION: Large elements, bold contrast, instant visual impact in 1.8 seconds.
DO NOT place text in bottom-right corner (YouTube timestamp overlay position).
DO NOT add more than 2 focal points — clutter kills CTR.
```

**design_type según plataforma:**
- YouTube → `youtube_thumbnail`
- Instagram feed → `instagram_post`
- Pinterest → `pinterest_pin`
- Stories → `your_story`
- Twitter/X → `twitter_post`

---

### FASE 4: TEST DE CALIDAD ANTES DE PRESENTAR

Para cada candidato generado, aplica mentalmente:

**TEST DE 1.8 SEGUNDOS:**
- [ ] ¿Se entiende el tema en menos de 2 segundos?
- [ ] ¿El elemento principal es lo primero que ve el ojo?
- [ ] ¿El texto es legible al 10% del tamaño real (miniatura en feed)?

**TEST DE CONTRASTE:**
- [ ] ¿El texto contrasta suficientemente con el fondo?
- [ ] ¿Hay contraste incluso en escala de grises?
- [ ] ¿Funciona en móvil con brillo bajo?

**TEST DE REGLAS:**
- [ ] ¿Hay texto en la esquina inferior derecha? (si sí → fallo crítico)
- [ ] ¿Hay más de 2 focos de atención? (si sí → simplificar)
- [ ] ¿Hay más de 5 palabras de texto? (si sí → reducir)

Informa al usuario si algún candidato falla un test crítico.

---

### FASE 5: SELECCIÓN Y EXPORTACIÓN

1. Presenta candidatos describiendo en 1 línea qué diferencia a cada uno
2. Usuario elige → `create-design-from-candidate`
3. Exportar → `export-design`
4. Recomendar A/B test si YouTube: subir 2 variaciones y comparar CTR en las primeras 48h

---

### FASE 6: ITERACIÓN INTELIGENTE

- **Expresión/composición débil** → Ajustar descripción del sujeto, añadir más especificidad emocional
- **Colores no destacan** → Cambiar a combinación de mayor contraste, añadir saturación
- **Texto no legible** → Aumentar tamaño, cambiar color, añadir sombra o backdrop
- **CTR bajo tras publicar** → Analizar qué variación A/B ganó y extraer el patrón
- Máx 3 iteraciones completas → Si no funciona, cambiar enfoque psicológico completamente

---

## REGLAS ABSOLUTAS

1. **SIEMPRE investigar antes de generar** (Fases 1A + 1B). Sin datos = thumbnail genérico.
2. **SIEMPRE generar en Canva**. Este skill termina con un diseño real, no con texto.
3. **SIEMPRE 3 variaciones** con enfoques distintos. El usuario elige con opciones reales.
4. **NUNCA texto en zona inferior derecha** — el timestamp de YouTube lo cubre.
5. **NUNCA más de 5 palabras** de texto en el thumbnail.
6. **NUNCA más de 2 focos de atención** — el clutter destruye el CTR.
7. **SIEMPRE aplicar el test de 1.8 segundos** antes de presentar candidatos.
8. **El texto amplifica curiosidad, nunca resume el vídeo.**
9. Expresiones faciales genuinas y relatables > expresiones teatrales exageradas.
