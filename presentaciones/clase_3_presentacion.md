# Clase 3: Pensamiento Computacional

## Innovación Tecnológica | Diseño de Videojuegos | Grados 6° - 10°
### Duración: 50 minutos | Sala de sistemas

---

# Parte 1: Repaso (5 min)

## ¿Qué hicimos la clase pasada?

- Elegimos la idea del juego
- Instalamos las herramientas
- Creamos nuestro primer proyecto

**¿Quién puede contar qué hace su juego?**
- 2-3 grupos comparten brevemente

---


# Parte 2: ¿Qué es el pensamiento computacional? (10 min)

## Definición simple

> "El **pensamiento computacional** es una forma de resolver problemas dividiéndolos en pasos pequeños y claros que una computadora puede seguir."

## ¿Por qué importa para videojuegos?

| Sin pensamiento computacional | Con pensamiento computacional |
|------------------------------|------------------------------|
| "El enemigo me persigue" | "El enemigo detecta mi posición, calcula la dirección, y se mueve hacia mí" |
| "El jugador salta" | "Cuando presiono espacio, el personaje sube y luego baja por gravedad" |
| "Pierdo una vida" | "Si toco un enemigo, restar 1 a vidas y reposicionar al jugador" |

## Las 4 habilidades

| Habilidad | Qué es | Ejemplo en videojuegos |
|-----------|--------|------------------------|
| **Descomposición** | Dividir un problema grande en partes pequeñas | Un juego = personajes + niveles + reglas + interfaz |
| **Reconocimiento de patrones** | Encontrar similitudes entre problemas | El mismo enemigo aparece en varios niveles |
| **Abstracción** | Ignorar detalles innecesarios | Un personaje es solo posición + imagen + vidas |
| **Algoritmos** | Crear instrucciones paso a paso | Si toco moneda → sumar puntos → eliminar moneda |

---

# Parte 3: Descomposición en acción (8 min)

## Actividad: Descomponer un juego

**Ejemplo con Mario Bros:**

```
JUEGO COMPLETO
├── Personajes
│   ├── Mario (jugador)
│   ├── Goombas (enemigos)
│   └── Bowser (jefe final)
├── Mundo
│   ├── Nivel 1-1
│   ├── Nivel 1-2
│   └── Nivel 1-3
├── Mecánicas
│   ├── Saltar
│   ├── Correr
│   └── Disparar (con power-up)
├── Interfaz
│   ├── Puntos
│   ├── Vidas
│   └── Tiempo
└── Reglas
    ├── Tocar enemigo = perder vida
    ├── Tocar bandera = ganar nivel
    └── Vidas = 0 = game over
```

## Ahora ustedes (5 min)

**En grupos, descompongan su juego:**

1. Escriban los **personajes principales**
2. Escriban los **escenarios/ubicaciones**
3. Escriban las **mecánicas básicas**
4. Escriban las **reglas** del juego

---

# Parte 4: Introducción a algoritmos (10 min)

## ¿Qué es un algoritmo?

> "Un **algoritmo** es una secuencia de instrucciones paso a paso para resolver un problema."

## Ejemplo: Algoritmo para caminar

```
1. Pararse
2. Mirar hacia el destino
3. Repetir hasta llegar:
   a. Dar un paso adelante
   b. Si hay obstáculo:
      - Esquivar a la derecha o izquierda
4. Detenerse
```

## Algoritmos en videojuegos

**Ejemplo: ¿Qué pasa cuando el jugador salta?**

| Paso | Instrucción |
|------|-------------|
| 1 | Detectar que se presionó la barra espaciadora |
| 2 | Verificar que el jugador está en el suelo |
| 3 | Cambiar la velocidad vertical hacia arriba |
| 4 | Aplicar gravedad cada frame |
| 5 | Cuando toque el suelo, detener la caída |

**Ejemplo: ¿Qué pasa cuando toco una moneda?**

| Paso | Instrucción |
|------|-------------|
| 1 | Detectar colisión entre jugador y moneda |
| 2 | Sumar 10 puntos al puntaje |
| 3 | Reproducir sonido de moneda |
| 4 | Eliminar la moneda de la pantalla |

---

# Parte 5: Práctica - Primeros algoritmos (12 min)

## Actividad en la herramienta

**Grado 6° - Scratch:**

| Paso | Acción |
|------|--------|
| 1 | Abrir proyecto creado |
| 2 | Ir a "Eventos" → arrastrar "Al presionar bandera verde" |
| 3 | Ir a "Movimiento" → arrastrar "mover 10 pasos" |
| 4 | Ir a "Apariencia" → arrastrar "decir Hola! por 2 segundos" |
| 5 | Probar haciendo click en la bandera verde |

**Grado 7° - GDevelop:**

| Paso | Acción |
|------|--------|
| 1 | Abrir proyecto creado |
| 2 | Crear un objeto "Jugador" |
| 3 | Agregar evento: "Al inicio de la escena" |
| 4 | Agregar acción: "Crear objeto Jugador en posición (400, 300)" |
| 5 | Probar la escena |

**Grados 8°, 9° y 10° - Godot:**

| Paso | Acción |
|------|--------|
| 1 | Abrir proyecto creado |
| 2 | Crear escena nueva |
| 3 | Agregar nodo "Sprite2D" |
| 4 | En el Inspector, asignar una textura |
| 5 | Guardar escena y ejecutar (F6) |

---

# Parte 6: Cierre (5 min)

## Resumen de hoy

| Concepto | Aprendimos |
|----------|------------|
| **Pensamiento computacional** | Resolver problemas dividiéndolos en pasos |
| **Descomposición** | Dividir en partes pequeñas |
| **Algoritmos** | Instrucciones paso a paso |
| **Práctica** | Primeros pasos en la herramienta |

## Tarea para la próxima clase

**Escriban 3 algoritmos de su juego:**

1. **Algoritmo de movimiento** del personaje principal
2. **Algoritmo de colisión** con un objeto (moneda, enemigo, etc.)
3. **Algoritmo de victoria/derrota** (¿qué pasa cuando ganas o pierdes?)

**Formato:**
```
ALGORITMO: [Nombre del algoritmo]
1. [Paso 1]
2. [Paso 2]
3. [Paso 3]
...
```

**Ejemplo:**
```
ALGORITMO: Recoger moneda
1. Detectar que el jugador toca la moneda
2. Sumar 10 puntos
3. Reproducir sonido
4. Hacer desaparecer la moneda
```

---

# Notas para el Docente

## Materiales necesarios:
- Computadores con las herramientas instaladas
- Proyector para ejemplos
- Hojas para algoritmos (opcional)

## Tiempos sugeridos:
| Parte | Tiempo | Actividad |
|-------|--------|-----------|
| 1 | 5 min | Repaso |
| 2 | 10 min | Pensamiento computacional |
| 3 | 8 min | Descomposición |
| 4 | 10 min | Algoritmos |
| 5 | 12 min | Práctica |
| 6 | 5 min | Cierre |

## Tips:
- Si algunos terminan rápido, pedirles que ayuden a compañeros
- La práctica puede extenderse si hay dudas
- Los algoritmos pueden ser más simples para grado 6°
- Verificar que todos lograron crear algo en la herramienta

## Diferenciación por grado:
| Grado | Complejidad de algoritmos |
|-------|--------------------------|
| 6° | 3-4 pasos, verbos simples |
| 7° | 4-5 pasos, condiciones simples |
| 8° | 5-6 pasos, condiciones y bucles |
| 9° | 6-8 pasos, lógica completa |
| 10° | 6-8 pasos, lógica completa, mayor profundidad en implementación |