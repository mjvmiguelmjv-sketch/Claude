# Sistema de Diseño Automatizado — Claude Code

Este repositorio contiene un sistema de skills para generar miniaturas y carruseles de alta conversión de forma automatizada, con investigación previa integrada.

## Skills disponibles

### `/thumbnail` — Generador de Miniaturas
Genera miniaturas optimizadas para máximo CTR en YouTube, Instagram, Pinterest y otras plataformas.

**Flujo:**
1. Investigación web de miniaturas exitosas en el nicho (WebSearch)
2. Extracción de patrones visuales y psicológicos
3. Construcción de brief detallado
4. Generación con Canva (generate-design)
5. Selección y exportación

**Uso mínimo:** `/thumbnail youtube "mi tema"`

---

### `/carousel` — Generador de Carruseles
Genera carruseles estructurados y visualmente cohesivos para Instagram, LinkedIn, Pinterest y más.

**Flujo:**
1. Investigación web de carruseles virales en el nicho (WebSearch)
2. Planificación de estructura slide a slide
3. Aprobación de estructura por el usuario
4. Generación con Canva (generate-design / generate-design-structured)
5. Selección y exportación

**Uso mínimo:** `/carousel instagram "mi tema"`

---

## Principios del sistema

- **Investigación primero, siempre.** Nunca se genera un diseño sin haber investigado qué funciona en el nicho.
- **El usuario solo pone las condiciones.** El sistema hace el resto: investiga, planifica, diseña.
- **Iteración guiada.** Si el resultado no satisface, el sistema ajusta inteligentemente.
- **Basado en datos reales.** Cada decisión de diseño está fundamentada en patrones de contenido exitoso.

---

## Herramientas del sistema

| Herramienta | Propósito |
|-------------|-----------|
| `WebSearch` | Investigación de tendencias y patrones exitosos |
| `generate-design` | Generación visual en Canva |
| `generate-design-structured` | Generación de presentaciones/carruseles estructurados |
| `create-design-from-candidate` | Convertir candidato en diseño editable |
| `export-design` | Exportar el diseño final |
| `start-editing-transaction` + `perform-editing-operations` | Ediciones puntuales post-generación |
| `list-brand-kits` | Aplicar branding del usuario |

---

## Ejemplo de sesión típica

```
Usuario: /thumbnail youtube "cómo ahorrar dinero en 2025" audiencia 25-35 años, estilo moderno

Sistema:
1. [Investiga] Busca patrones en miniaturas de finanzas personales exitosas
2. [Resume] Presenta hallazgos: colores verdes/negros, cara expresiva, texto "AHORRA X€"
3. [Genera] Crea 3 candidatos en Canva con brief detallado
4. [Selección] Usuario elige candidato 2
5. [Exporta] Descarga lista para subir
```
