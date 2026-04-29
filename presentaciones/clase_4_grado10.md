# Clase 4 - Grado 10: Estructura del Game Design Document (GDD)

**Duración:** 50 minutos  
**Sala:** Sala de sistemas  
**Objetivo:** Comprender la estructura profesional de un GDD y comenzar a documentar el videojuego

---

## ¿Qué es un GDD?

El **Game Design Document** es la "biblia" de tu videojuego. Contiene TODO lo que necesitas saber para crearlo.

**Propósitos:**
- 📋 Planificar antes de programar
- 🤝 Alinear al equipo (¡no peleen por decisiones ya tomadas!)
- 📝 Referencia durante el desarrollo
- 🎯 Evitar el "scope creep" (el juego se hace gigante sin control)

---

## Estructura de un GDD Profesional

```
GAME DESIGN DOCUMENT: [Nombre del Juego]

═══════════════════════════════════════════════════════

1. VISIÓN GENERAL
   ├── Título (tentativo)
   ├── Género
   ├── Plataforma(s)
   ├── Público objetivo
   └── Resumen ejecutivo (elevator pitch)

2. HISTORIA Y NARRATIVA
   ├── Sinopsis
   ├── Personajes principales
   ├── Ambientación (mundo, época)
   └── Arco narrativo

3. MECÁNICAS DE JUEGO
   ├── Controles
   ├── Movimiento del jugador
   ├── Sistema de combate/interacción
   ├── Power-ups y objetos
   └── Reglas del juego

4. DISEÑO DE NIVELES
   ├── Estructura (lineal, abierto, por mundos)
   ├── Progresión de dificultad
   └── Lista de niveles con descripción

5. ARTE Y ESTILO VISUAL
   ├── Estilo (pixel art, 2D, 3D, cartoon, realista)
   ├── Personajes (descripción visual)
   ├── Escenarios
   └── Referencias visuales (mood board)

6. AUDIO
   ├── Música (ambientación, temas)
   ├── Efectos de sonido
   └── Diálogos (si aplica)

7. INTERFAZ DE USUARIO (UI)
   ├── HUD (lo que se ve jugando)
   ├── Menús (principal, pausa, opciones)
   └── Iconos y botones

8. ASSETS REQUERIDOS
   ├── Lista de sprites/modelos
   ├── Lista de sonidos
   └── Lista de animaciones

9. CRONOGRAMA
   ├── Hitos principales
   └── Responsables por tarea
```

---

## Estructura de la Clase

### 1. Presentación de la Estructura (15 minutos)
- Revisar cada sección del GDD
- Ver ejemplos de GDDs reales (fragmentos)

### 2. Taller: Comenzar el GDD (30 minutos)

**Actividad:** Completen las secciones 1, 2 y 8 de su GDD

```markdown
# GDD - [Nombre del Juego]
**Grupo:** [Nombres]
**Fecha:** [Fecha]

---

## 1. VISIÓN GENERAL

**Título:** [Nombre tentativo]

**Género:** [Género + subgénero]

**Plataforma:** Godot Engine 4 → Exportar a [Web/PC]

**Público objetivo:**
- Edad: [X-X años]
- Tipo de jugador: [casual/medio/hardcore]
- Preferencias: [qué tipo de juegos les gustan]

**Resumen ejecutivo (elevator pitch):**
[3-4 oraciones que venden tu juego]

---

## 2. HISTORIA Y NARRATIVA

**Sinopsis:**
[2-3 párrafos contando la historia]

**Personaje Principal:**
- Nombre:
- Descripción física:
- Personalidad:
- Habilidad especial:

**Antagonista/Villano:**
- Nombre:
- Motivación:
- Cómo se enfrenta al jugador:

**Ambientación:**
- ¿Dónde ocurre?
- ¿Cuándo ocurre?
- ¿Qué hace especial este mundo?

---

## 8. ASSETS REQUERIDOS (lista inicial)

**Sprites/Modelos:**
- [ ] Personaje principal
- [ ] Enemigo 1
- [ ] Enemigo 2
- [ ] Escenario base
- [ ] Objetos coleccionables
- [ ] Jefe final

**Sonidos:**
- [ ] Música de fondo
- [ ] Salto
- [ ] Daño
- [ ] Victoria
- [ ] Derrota

**Animaciones:**
- [ ] Idle (quieto)
- [ ] Correr
- [ ] Saltar
- [ ] Atacar
- [ ] Morir
```

### 3. Cierre y Tarea (5 minutos)
- Guardar en: `grado_10/grupo_[nombre]/gdd_v1.md`
- Tarea: Pensar en referencias visuales para la próxima clase

---

## Entregable

- **Archivo:** `grado_10/grupo_[nombre]/gdd_v1.md`
- Secciones 1, 2 y 8 completas

---

## Rúbrica

| Criterio | Excelente (5) | Bueno (4) | Regular (3) |
|----------|---------------|-----------|-------------|
| Visión clara | Se entiende el juego perfectamente | Mayormente claro | Vago o confuso |
| Narrativa | Historia con sentido y motivación | Historia básica | Sin historia definida |
| Completitud | Todas las secciones respondidas | Faltan detalles | Incompleto |
| Formato | Limpio, organizado, profesional | Algunos errores | Desordenado |
