# Clase 5 - Grado 6: Diagramas de Flujo para Videojuegos

**Duración:** 50 minutos  
**Sala:** Sala de sistemas  
**Objetivo:** Representar visualmente algoritmos usando diagramas de flujo

---

## ¿Qué es un Diagrama de Flujo?

Es una representación **gráfica** de un algoritmo o proceso. Usa símbolos conectados por flechas para mostrar el orden de las acciones.

### Símbolos Básicos

```
┌─────────────┐
│   ÓVALO     │ → INICIO / FIN
│  (Inicio)   │
└─────────────┘

┌─────────────┐
│  RECTÁNGULO │ → ACCIÓN / PROCESO
│  (acción)   │
└─────────────┘

┌─────────────┐
│   ROMBO     │ → DECISIÓN (Sí/No)
│  (¿condición?)│
└─────────────┘

┌─────────────┐
│ PARALELOGRAMO│ → ENTRADA / SALIDA
│  (datos)    │
└─────────────┘

     ↓
   FLECHA    → DIRECCIÓN DEL FLUJO
```

---

## Estructura de la Clase

### 1. Introducción (10 minutos)
- Mostrar ejemplos de diagramas de flujo simples
- Explicar cada símbolo y su uso

### 2. Ejemplo Guiado: "Saltar en un Juego" (10 minutos)

```
     [INICIO]
        ↓
  ¿Botón presionado?
     /       \
   NO        SÍ
    ↓         ↓
 [Esperar]  ¿En el suelo?
              /    \
            NO      SÍ
             ↓       ↓
         [Esperar]  [Aplicar fuerza hacia arriba]
                         ↓
                   [Personaje sube]
                         ↓
                   ¿Altura máxima?
                       /    \
                     NO      SÍ
                      ↓       ↓
                   [Seguir]  [Empezar a caer]
                                 ↓
                            ¿Tocó suelo?
                               /   \
                             NO     SÍ
                              ↓      ↓
                           [Cayendo] [FIN salto]
```

### 3. Actividad Principal (25 minutos)

**Instrucciones:**
1. Tomen el algoritmo que hicieron en la clase 4
2. Conviértanlo en un diagrama de flujo
3. Pueden usar:
   - Papel y lápiz (foto al final)
   - Herramienta digital: [draw.io](https://app.diagrams.net/) (gratis, sin login)

**Pasos en draw.io:**
1. Entrar a la web
2. Elegir "Create new diagram"
3. Seleccionar "Flowchart"
4. Arrastrar símbolos desde la izquierda
5. Conectar con flechas
6. Exportar como imagen o PDF

### 4. Cierre (5 minutos)
- Guardar el diagrama en: `grado_6/grupo_[nombre]/diagrama_clase5.png` (o .pdf)

---

## Entregable

- **Archivo:** `grado_6/grupo_[nombre]/diagrama_clase5.png` (o formato de imagen/pdf)
- Diagrama de flujo del algoritmo de la clase 4

---

## Rúbrica

| Criterio | Excelente (5) | Bueno (4) | Regular (3) |
|----------|---------------|-----------|-------------|
| Símbolos correctos | Todos los símbolos bien usados | 1-2 errores | Muchos errores |
| Flujo lógico | Se sigue fácilmente | Algunas confusiones | Difícil de seguir |
| Completitud | Cubre todo el algoritmo | Faltan partes | Incompleto |
| Claridad visual | Limpio y organizado | Algo desordenado | Confuso |

---

## Tips

✅ Usen texto CORTO dentro de cada símbolo  
✅ Las flechas deben ir en dirección lógica (arriba→abajo o izquierda→derecha)  
✅ Para decisiones, etiquetar las salidas con "SÍ" y "NO"  
❌ No crucen flechas innecesariamente  
❌ No usen el mismo símbolo para cosas diferentes
