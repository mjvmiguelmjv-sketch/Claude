# Skill: /carousel — Generador de Carruseles con Investigación Previa

## Propósito
Genera carruseles de alta engagement para Instagram, LinkedIn, Pinterest u otras plataformas, investigando primero las estructuras y estilos que mejor funcionan en el nicho del usuario.

---

## Cómo invocar este skill

```
/carousel [plataforma] [tema/nicho] [condiciones opcionales]
```

**Ejemplos:**
- `/carousel instagram "productividad" 7 slides, estilo minimalista, tipografía bold`
- `/carousel linkedin "liderazgo empresarial" 5 slides, tono profesional, colores corporativos`
- `/carousel instagram "recetas fitness" 6 slides, colores vibrantes, mucho visual`

Si el usuario no proporciona suficiente contexto, PREGUNTA antes de continuar:
1. ¿Para qué plataforma? (Instagram, LinkedIn, Pinterest, Facebook)
2. ¿Cuál es el tema del carrusel?
3. ¿Cuántas diapositivas? (recomendado: 5-10)
4. ¿Hay condiciones especiales? (estilo, tono, colores, si lleva portada especial, CTA final)

---

## Proceso de ejecución — SEGUIR EN ORDEN ESTRICTO

### FASE 1: INVESTIGACIÓN (obligatoria, no saltarse nunca)

1. Usa `WebSearch` para investigar carruseles exitosos en el nicho. Ejecuta **al menos 3 búsquedas**:
   - `"[tema] carousel instagram high engagement 2024 2025"`
   - `"[nicho] carousel design structure best practices [plataforma]"`
   - `"[tema] swipe post viral formula hook"`

2. Extrae y documenta los **patrones de éxito**:
   - **Estructura narrativa**: ¿Cómo arranca el carrusel? ¿Hook de problema? ¿Promesa de valor? ¿Datos impactantes?
   - **Slide de portada (cover)**: ¿Qué elementos tiene? ¿Título + número? ¿Pregunta?
   - **Estructura interna**: ¿Una idea por slide? ¿Paso a paso? ¿Lista numerada? ¿Pregunta-respuesta?
   - **Slide de cierre (CTA)**: ¿Qué tipo de llamada a la acción se usa?
   - **Estilo visual**: ¿Minimalista? ¿Con ilustraciones? ¿Solo tipografía? ¿Fotografía?
   - **Paleta**: ¿Colores consistentes? ¿Un color de acento por slide o toda la misma paleta?
   - **Tipografía**: ¿Bold para títulos? ¿Contraste fuerte? ¿Texto corto o párrafos?

3. Presenta al usuario el **resumen de investigación**:

```
## Investigación completada para: [tema] en [plataforma]

### Patrones identificados en carruseles exitosos:
- Estructura ganadora: [hallazgos]
- Cover/portada: [hallazgos]
- Desarrollo interno: [hallazgos]
- CTA final: [hallazgos]
- Estilo visual dominante: [hallazgos]
- Paleta de colores: [hallazgos]

### Estrategia recomendada para tu carrusel:
[Breve párrafo explicando el enfoque y por qué funcionará]
```

---

### FASE 2: PLANIFICACIÓN DEL CONTENIDO

Antes de diseñar, define el **esqueleto del carrusel**. Presenta al usuario la estructura slide a slide:

```
## Estructura propuesta del carrusel: "[Título del carrusel]"

SLIDE 1 — PORTADA (Cover):
Título: [texto impactante]
Subtítulo: [frase de apoyo opcional]
Visual: [descripción]

SLIDE 2:
Título: [texto del slide]
Contenido: [copy breve]

SLIDE 3:
...

SLIDE [N] — CIERRE (CTA):
Mensaje: [llamada a la acción]
Visual: [descripción]
```

**Pregunta al usuario si aprueba la estructura** antes de continuar a generación.
Si pide cambios, ajusta el esqueleto y vuelve a mostrar antes de generar.

---

### FASE 3: GENERACIÓN CON CANVA

Una vez aprobada la estructura, genera el diseño.

**Estrategia de generación para carruseles:**

Para carruseles en Canva usa `generate-design` con `design_type: presentation` para obtener múltiples slides cohesivos. Alternativamente, si son posts individuales tipo carrusel de Instagram, usa `instagram_post` con un query que describa el sistema visual completo.

**Estructura del query ideal para carrusel:**
```
[Número] slide carousel for [plataforma] about [tema].
Slide 1 cover: [descripción portada].
Internal slides: [descripción de estilo general y elementos].
Final slide CTA: [descripción cierre].
Visual style: [estilo]. Color palette: [colores].
[Tipografía]. Professional, engaging, optimized for [plataforma].
High contrast, consistent branding across all slides.
```

Construye el query con el máximo detalle posible, incluyendo el contenido clave de cada slide.

**Si se usa `generate-design-structured` para presentaciones:**
- Llena `presentation_outlines` con cada slide (title + description)
- `topic`: el tema del carrusel
- `audience`: el público objetivo
- `style`: el estilo visual determinado por la investigación
- `length`: número de slides

---

### FASE 4: PRESENTACIÓN Y SELECCIÓN

1. Muestra los candidatos generados
2. Pregunta cuál prefiere
3. Si selecciona uno, usa `create-design-from-candidate` para hacerlo editable
4. Pregunta si quiere exportarlo con `export-design`

---

### FASE 5: ITERACIÓN (si aplica)

Si el usuario no está satisfecho:
- Identifica qué slide o elemento cambiar
- Ajusta el query o usa `start-editing-transaction` + `perform-editing-operations` para ediciones puntuales
- Si el cambio es global de estilo, regenera con query mejorado

---

## Tipos de carrusel y cuándo usar cada design_type

| Tipo de carrusel | Plataforma | design_type recomendado |
|-----------------|------------|------------------------|
| Carrusel swipe educativo | Instagram | `presentation` o `instagram_post` |
| Carrusel profesional | LinkedIn | `presentation` |
| Infografía por partes | Instagram/Pinterest | `infographic` o `pinterest_pin` |
| Story secuencial | Instagram/TikTok | `your_story` |
| Post único tipo carrusel | Facebook | `facebook_post` |

---

## Reglas del sistema

- **NUNCA generar sin investigar primero**. La investigación define la estructura ganadora.
- **NUNCA saltar la aprobación de estructura**. El usuario debe ver el esqueleto antes de generarse el diseño.
- El copy de cada slide debe ser **concreto y breve**: máximo 15-20 palabras por slide visible.
- La portada (slide 1) es el elemento más importante: debe generar el "swipe" inmediato.
- El CTA final siempre debe tener una acción clara: "Guarda este post", "Sigue para más", "Comenta X".
- Si el usuario pide más de 10 slides, recomiéndale dividir en 2 carruseles para mantener engagement.
- Mantén coherencia visual entre todos los slides: misma paleta, misma tipografía, mismo estilo.
