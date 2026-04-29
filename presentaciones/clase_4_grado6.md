# Clase 4 - Grado 6: Algoritmos y Secuencias

**Duración:** 50 minutos  
**Sala:** Sala de sistemas  
**Objetivo:** Comprender qué es un algoritmo y cómo aplicarlo al diseño de videojuegos

---

## Estructura de la Clase

### 1. Introducción (5 minutos)
- ¿Qué es un algoritmo? Una serie de pasos para resolver un problema
- Ejemplo cotidiano: receta de cocina, instrucciones para llegar a un lugar
- En videojuegos: cada acción del personaje sigue un algoritmo

### 2. Actividad Principal - "El Algoritmo de mi Juego" (35 minutos)

**Instrucciones:**
1. En parejas, elijan UNA mecánica de su videojuego (ej: saltar, recoger moneda, esquivar obstáculo)
2. Descompongan esa mecánica en pasos específicos
3. Escriban el algoritmo usando esta estructura:

```
ALGORITMO: [Nombre de la mecánica]

PASOS:
1. [Primera acción]
2. [Segunda acción]
3. [Tercera acción]
...

CONDICIONES:
- SI [condición] ENTONCES [acción]
- SI NO [acción alternativa]

REPETIR:
- MIENTRAS [condición] HACER [acción repetitiva]
```

**Ejemplo completo:**
```
ALGORITMO: Saltar obstáculo

PASOS:
1. Jugador presiona botón de saltar
2. Personaje se mueve hacia arriba
3. Personaje alcanza altura máxima
4. Personaje cae al suelo

CONDICIONES:
- SI personaje está en el aire ENTONCES no puede saltar de nuevo
- SI personaje toca obstáculo ENTONCES pierde una vida

REPETIR:
- MIENTRAS botón esté presionado HACER verificar posición
```

### 3. Puesta en Común (10 minutos)
- 2-3 grupos comparten su algoritmo
- Discusión: ¿Qué condiciones son importantes? ¿Qué pasa si olvidamos un caso?

---

## Entregable de la Clase

Cada grupo debe tener escrito en su carpeta:
- **Archivo:** `grado_6/grupo_[nombre]/algoritmo_clase4.md`
- Contenido: Algoritmo completo de UNA mecánica de su juego

---

## Rúbrica de Evaluación

| Criterio | Excelente (5) | Bueno (4) | Regular (3) |
|----------|---------------|-----------|-------------|
| Claridad de pasos | Pasos lógicos y ordenados | Pasos comprensibles | Pasos confusos |
| Condiciones | Usa SI-ENTONCES correctamente | Intenta usar condiciones | Sin condiciones |
| Completitud | Cubre todos los casos | Cubre la mayoría | Faltan casos importantes |

---

## Tarea para la próxima clase

Pensar en cómo representarían su algoritmo visualmente (dibujos, símbolos, flechas).
