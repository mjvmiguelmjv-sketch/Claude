---
name: thumbnail
description: Genera miniaturas de alta conversión para YouTube, Instagram, Pinterest y otras plataformas. Investiga primero qué está funcionando en el nicho y luego genera el diseño perfecto con Canva. Úsalo cuando el usuario quiera crear una miniatura, thumbnail o imagen de portada para contenido.
---

# Skill: /thumbnail — Generador de Miniaturas con Investigación Previa

## Propósito
Genera miniaturas de alta conversión para YouTube, Instagram, LinkedIn u otras plataformas, realizando primero una investigación profunda de lo que está funcionando en el nicho del usuario.

---

## Cómo invocar este skill

```
/thumbnail [plataforma] [tema/nicho] [condiciones opcionales]
```

**Ejemplos:**
- `/thumbnail youtube "marketing digital" audiencia jóvenes empresarios, colores oscuros`
- `/thumbnail instagram "fitness" sin cara, estilo minimalista`
- `/thumbnail youtube "tecnología IA" clickbait emocional, texto grande`

Si el usuario no proporciona suficiente contexto, PREGUNTA antes de continuar:
1. ¿Para qué plataforma? (YouTube, Instagram, LinkedIn, Pinterest, Twitter/X)
2. ¿Cuál es el tema principal del contenido?
3. ¿Hay alguna condición especial? (estilo, colores, sin cara, con texto específico, emociones, etc.)

---

## Proceso de ejecución — SEGUIR EN ORDEN ESTRICTO

### FASE 1: INVESTIGACIÓN (obligatoria, no saltarse nunca)

1. Usa `WebSearch` para buscar miniaturas exitosas en el nicho. Ejecuta **al menos 3 búsquedas** diferentes:
   - `"[tema] YouTube thumbnail best performing 2024 2025"`
   - `"[tema] thumbnail design psychology high CTR"`
   - `"[nicho] viral thumbnail formula [plataforma]"`

2. Con los resultados, extrae y documenta en tu respuesta los **patrones que más se repiten**:
   - **Colores dominantes**: ¿Fondos oscuros o claros? ¿Qué colores de acento?
   - **Tipografía**: ¿Texto grande y corto? ¿Menos de 5 palabras? ¿Fuentes de palo seco?
   - **Composición**: ¿Cara con expresión exagerada? ¿Fondo simple? ¿Objetos llamativos?
   - **Emociones**: ¿Sorpresa, miedo, curiosidad, deseo?
   - **Fórmulas textuales**: ¿"Nunca…", "Secreto de…", números grandes, preguntas?
   - **Elementos visuales recurrentes**: flechas, círculos de énfasis, miniaturas de estilo "shock"

3. Presenta al usuario un **resumen de investigación** en este formato:

```
## Investigación completada para: [tema] en [plataforma]

### Patrones identificados en miniaturas exitosas:
- Colores: [hallazgos]
- Tipografía: [hallazgos]
- Composición: [hallazgos]
- Emociones predominantes: [hallazgos]
- Fórmulas de texto: [hallazgos]

### Estrategia recomendada para tu miniatura:
[Breve párrafo explicando el enfoque]
```

---

### FASE 2: CONSTRUCCIÓN DEL BRIEF

Con la investigación + las condiciones del usuario, crea un **brief detallado** para la generación. El brief debe incluir:

- **Tipo**: `youtube_thumbnail` o el tipo correcto para la plataforma
- **Tema visual principal**: qué debe verse en primer plano
- **Paleta de colores**: colores específicos con justificación
- **Texto en la miniatura**: máximo 5-6 palabras, impacto máximo
- **Estilo**: moderno, minimalista, shock, lifestyle, editorial, etc.
- **Emoción objetivo**: la emoción que debe transmitir al espectador
- **Elementos de apoyo**: iconos, flechas, efectos, gradientes

---

### FASE 3: GENERACIÓN CON CANVA

Usa el tool `generate-design` con:
- `design_type`: `youtube_thumbnail` (o `instagram_post`, `pinterest_pin`, `your_story` según plataforma)
- `query`: Un prompt rico y detallado construido desde el brief. **Nunca usar prompts genéricos.** El prompt debe ser específico, descriptivo y orientado al CTR.

**Estructura del query ideal:**
```
[Estilo visual] YouTube thumbnail for [tema].
[Paleta de colores] with [texto principal en miniatura].
[Composición: qué hay en primer plano, segundo plano].
[Emoción]. [Elementos visuales].
High contrast, bold typography, professional and eye-catching.
```

Genera siempre con el máximo detalle posible en el query.

---

### FASE 4: PRESENTACIÓN Y SELECCIÓN

1. Muestra los candidatos generados al usuario
2. Pregunta cuál prefiere
3. Si el usuario selecciona uno, usa `create-design-from-candidate` para convertirlo en diseño editable
4. Pregunta si quiere exportarlo con `export-design`

---

### FASE 5: ITERACIÓN (si aplica)

Si el usuario no está satisfecho:
- Pregunta qué cambiar específicamente
- Ajusta el brief
- Regenera con `generate-design` con el query mejorado
- Máximo 3 iteraciones antes de preguntar si prefiere empezar de nuevo

---

## Reglas del sistema

- **NUNCA generar sin investigar primero**. La investigación es lo que diferencia una miniatura buena de una excelente.
- **NUNCA usar queries genéricos** como "YouTube thumbnail about marketing". Siempre específicos.
- Si el usuario da condiciones contradictorias con los patrones de investigación, **menciona el conflicto** y pregunta cómo proceder.
- Si la plataforma no es YouTube, adapta el `design_type` correctamente:
  - Instagram feed → `instagram_post`
  - Instagram/TikTok Stories → `your_story`
  - Pinterest → `pinterest_pin`
  - Twitter/X → `twitter_post`
  - LinkedIn → `facebook_post` (formato más cercano disponible)
- Siempre muestra el resumen de investigación ANTES de generar. No saltar al diseño directamente.
