# Clase 6 - Grado 9: Prototipo de Papel (Paper Prototype)

**Duración:** 50 minutos  
**Sala:** Sala de sistemas  
**Objetivo:** Crear y probar un prototipo físico del videojuego para validar mecánicas

---

## ¿Qué es un Prototipo de Papel?

Es una versión **FÍSICA** de tu juego que puedes probar SIN programar.

**Se usa para:**
- ✅ Validar mecánicas antes de gastar tiempo en código
- ✅ Encontrar problemas de diseño temprano
- ✅ Probar con jugadores reales rápidamente
- ✅ Iterar rápido (cambiar es solo redibujar)

**Empresas como Nintendo y Blizzard lo usan incluso hoy.**

---

## ¿Cómo se hace?

Depende del género:

### Para Plataformas
- Dibujar el nivel en papel cuadriculado
- Usar una ficha o moneda como personaje
- Mover manualmente según reglas escritas
- Contar turnos/acciones

### Para Puzzle
- Recortar piezas de papel
- Armar y desarmar el puzzle
- Cronometrar intentos

### Para Aventura/RPG
- Crear cartas de opciones
- Usar dados para aleatoriedad
- Hoja de personaje con stats

---

## Estructura de la Clase

### 1. Introducción y Ejemplos (10 minutos)
- Mostrar ejemplos de prototipos de papel exitosos
- Explicar el proceso de prueba

### 2. Creación del Prototipo (20 minutos)

**Materiales necesarios:**
- Papel (cuadriculado preferiblemente)
- Lápices de colores
- Tijeras
- Dados (o app de dados en el celular)
- Fichas/monedas para personajes

**Parte 1: Diseñar el Nivel/Escenario (10 min)**
- Dibujar 1 nivel completo en papel
- Marcar: inicio, obstáculos, enemigos, meta, coleccionables

**Parte 2: Crear las Reglas (10 min)**
- Escribir las reglas de movimiento
- Definir acciones por turno
- Establecer condiciones de victoria/derrota

```markdown
# REGLAS DEL PROTOTIPO

## Movimiento
- El jugador puede moverse [X] casillas por turno
- Saltar cuesta [X] acción(es)
- [Otras reglas de movimiento]

## Acciones
- [Acción 1]: [qué hace, cuándo se usa]
- [Acción 2]: [qué hace, cuándo se usa]

## Enemigos
- [Enemigo 1]: se mueve [X] casillas, ataca si [condición]
- [Enemigo 2]: se mueve [X] casillas, ataca si [condición]

## Victoria
- Ganas cuando: [condición]

## Derrota
- Pierdes cuando: [condición]
```

### 3. Prueba del Prototipo (15 minutos)

**Opción A: Intercambiar con otro grupo**
- Otro grupo juega TU prototipo
- Tú observas SIN explicar (si se confunden, es problema del diseño)
- Tomas notas de dónde se traban, qué preguntas hacen

**Opción B: Jugar entre ustedes**
- Un compañero juega, el otro observa
- Luego cambian

**Durante la prueba, el "jugador" debe:**
- Pensar en voz alta ("quiero hacer X, ¿puedo?")
- Decir cuándo se frustra o confunde
- Compartir qué le gusta

**Hoja de Observación:**

```markdown
# OBSERVACIÓN DE PRUEBA

**Jugador:** [Nombre]
**Fecha:** [Fecha]
**Nivel probado:** [Número/nombre]

## Métricas
- **Tiempo para completar:** [X minutos]
- **Errores/Equívocos:** [número de veces que se confundió]
- **Momentos de frustración:** [dónde y por qué]
- **Momentos de diversión:** [qué le gustó]

## Feedback del Jugador
**Lo que entendió:**
[Qué reglas/me c ánicas captó rápido]

**Lo que no entendió:**
[Dónde se confundió]

**Sugerencias:**
[Qué dijo que podría mejorar]

## Cambios a Realizar
1. [Cambio 1 basado en lo observado]
2. [Cambio 2]
3. [Cambio 3]
```

### 4. Iteración y Cierre (5 minutos)
- Discutir qué cambios harían basados en la prueba
- Guardar documentación en: `grado_9/grupo_[nombre]/prototipo_papel_clase6.md`
- Tomar foto del prototipo y guardar como `prototipo_foto.jpg`

---

## Entregable

- **Archivo:** `grado_9/grupo_[nombre]/prototipo_papel_clase6.md`
- Contenido:
  1. Reglas del prototipo
  2. Hoja de observación de prueba
  3. Lista de cambios a realizar
- **Foto:** `prototipo_foto.jpg` (foto del prototipo físico)

---

## Rúbrica

| Criterio | Excelente (5) | Bueno (4) | Regular (3) |
|----------|---------------|-----------|-------------|
| Prototipo | Nivel completo y jugable | Faltan partes | Incompleto o injugable |
| Reglas | Claras y consistentes | Algunas lagunas | Confusas o incompletas |
| Prueba | Probado con feedback documentado | Probado sin documentar | No probado |
| Iteración | 3+ cambios identificados | 1-2 cambios | Sin cambios identificados |

---

## Tips

✅ El prototipo debe ser JUGABLE (puedes terminar el nivel)  
✅ Observa MÁS de lo que explicas (si tienes que explicar, el diseño falló)  
✅ Anota TODO lo que dice el jugador (aunque parezca obvio)  
❌ No te enamores del diseño: si algo no funciona, CÁMBIALO  
❌ No necesita ser bonito: es funcional, no arte final

---

## Ejemplo: Prototipo de Plataformas en Papel

```
┌─────────────────────────────────────────────────────────┐
│  S = Inicio                                              │
│  E = Enemigo                                             │
│  M = Moneda                                              │
│  ^ = Pincho (muerte)                                     │
│  F = Final                                               │
│                                                          │
│  Nivel 1: "El Comienzo"                                  │
│                                                          │
│  S  →  M  →  M  →  E  →  M  →  ^  →  M  →  F            │
│              ↑                    ↑                      │
│              M                    ^                      │
│                                                          │
│  REGLAS:                                                 │
│  - Jugador mueve 1 casilla por turno (o 2 si corre)      │
│  - Saltar cuesta 1 acción                                │
│  - Enemigo mueve 1 casilla hacia el jugador cada 2 turnos│
│  - Recoger moneda: acción gratis                         │
│  - Tocar enemigo o pincho: vuelve al inicio              │
│  - Llegar a F: gana el nivel                             │
└─────────────────────────────────────────────────────────┘
```
