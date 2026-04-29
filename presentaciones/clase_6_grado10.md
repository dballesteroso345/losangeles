# Clase 6 - Grado 10: Mecánicas y Niveles del Videojuego

**Duración:** 50 minutos  
**Sala:** Sala de sistemas  
**Objetivo:** Diseñar las mecánicas principales y la estructura de niveles del videojuego

---

## ¿Qué es una Mecánica?

Una **mecánica** es una regla o sistema que define cómo funciona el juego.

**Ejemplos:**
- Saltar (mecánica de movimiento)
- Disparar (mecánica de combate)
- Recoger monedas (mecánica de colección)
- Vida/vidas (mecánica de salud)

---

## Tipos de Mecánicas

| Categoría | Ejemplos |
|-----------|----------|
| **Movimiento** | Caminar, correr, saltar, volar, teletransportarse |
| **Acción** | Atacar, usar objetos, hablar, construir |
| **Progresión** | Experiencia, niveles, desbloqueables |
| **Economía** | Monedas, tiendas, intercambio |
| **Combate** | Daño, defensa, habilidades especiales |
| **Puzzle** | Interruptores, patrones, lógica |

---

## Estructura de la Clase

### 1. Introducción: De la Idea a la Mecánica (10 minutos)
- Cómo traducir la narrativa a acciones jugables
- La importancia de que las mecánicas apoyen la historia

### 2. Taller de Diseño de Mecánicas (20 minutos)

**Parte 1: Lista de Mecánicas (10 min)**
Identifiquen TODAS las mecánicas que tendrá su juego:

```markdown
## MECÁNICAS DEL JUEGO

### Mecánicas Principales (core)
1. [Nombre]: [descripción en 1 oración]
2. [Nombre]: [descripción en 1 oración]
3. [Nombre]: [descripción en 1 oración]

### Mecánicas Secundarias
1. [Nombre]: [descripción]
2. [Nombre]: [descripción]

### Mecánicas de Progresión
1. [Cómo avanza el jugador]
2. [Cómo se mide el éxito]
```

**Parte 2: Detalle de Cada Mecánica (10 min)**
Para cada mecánica PRINCIPAL, completen:

```markdown
### [Nombre de la mecánica]

**¿Qué hace el jugador?**
[Acción concreta]

**¿Qué resultado produce?**
[Efecto en el juego]

**¿Qué teclas/botones usa?**
[Controles]

**¿Qué limita esta mecánica?**
[Cooldown, recursos, condiciones]

**¿Cómo se relaciona con otras mecánicas?**
[Conexiones]
```

### 3. Diseño de Niveles (15 minutos)

**Estructura de niveles:**
- ¿Cuántos niveles tendrá el juego?
- ¿Cómo se desbloquean?
- ¿Qué hace único a cada nivel?

```markdown
## ESTRUCTURA DE NIVELES

### Nivel 1: [Nombre]
**Tema:** [bosque, ciudad, espacio, etc.]
**Nueva mecánica que introduce:** [cuál]
**Desafío principal:** [qué debe superar el jugador]
**Recompensa:** [qué gana al completar]

### Nivel 2: [Nombre]
**Tema:** [...]
**Nueva mecánica que introduce:** [...]
**Desafío principal:** [...]
**Recompensa:** [...]

### Nivel 3: [Nombre]
[...]

### Jefe Final / Nivel Final
**Descripción:** [...]
**Condiciones de victoria:** [...]
```

### 4. Cierre (5 minutos)
- Guardar todo en: `grado_10/grupo_[nombre]/mecanicas_niveles_clase6.md`

---

## Entregable

- **Archivo:** `grado_10/grupo_[nombre]/mecanicas_niveles_clase6.md`
- Contenido:
  1. Lista completa de mecánicas
  2. Detalle de mecánicas principales (3 mínimo)
  3. Estructura de niveles (3 niveles mínimo)

---

## Rúbrica

| Criterio | Excelente (5) | Bueno (4) | Regular (3) |
|----------|---------------|-----------|-------------|
| Mecánicas | 5+ mecánicas bien definidas | 3-4 mecánicas | 1-2 mecánicas |
| Detalle | Cada mecánica fully especificada | Algo detalladas | Vagas |
| Niveles | 3+ niveles con identidad propia | 2 niveles | 1 nivel o genéricos |
| Coherencia | Mecánicas apoyan la narrativa | Algo conectadas | Desconectadas |

---

## Ejemplo de Mecánica Detallada

```markdown
### Salto con Propulsor

**¿Qué hace el jugador?**
Presiona espacio para saltar, y puede mantener presionado para usar el propulsor y subir más alto.

**¿Qué resultado produce?**
El personaje salta. Si mantiene el botón, el propulsor lo impulsa 2x más alto.

**¿Qué teclas/botones usa?**
- Espacio (saltar)
- Mantener espacio (propulsor)

**¿Qué limita esta mecánica?**
Barra de combustible que se gasta con el propulsor. Se recarga en el suelo.

**¿Cómo se relaciona con otras mecánicas?**
- Permite alcanzar plataformas altas (exploración)
- Se puede esquivar enemigos saltando (combate)
- Algunas zonas requieren el propulsor (progresión)
```

---

## Tips

✅ Las mecánicas deben ser FÁCILES de explicar  
✅ Cada nivel debe enseñar algo nuevo  
✅ El primer nivel debe ser el más fácil (curva de aprendizaje)  
❌ No agreguen mecánicas "porque sí" (deben tener propósito)  
❌ No diseñen niveles demasiado complejos para primer prototipo
