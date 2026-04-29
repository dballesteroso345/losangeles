# Clase 6 - Grado 11: Diagramas UML y de Flujo del Sistema

**Duración:** 50 minutos  
**Sala:** Sala de sistemas  
**Objetivo:** Crear diagramas UML que documenten la arquitectura del sistema

---

## ¿Qué es UML?

**UML = Unified Modeling Language**

Es un lenguaje visual para modelar sistemas de software. Sirve para:
- 📐 Documentar la arquitectura antes de programar
- 🤝 Comunicar el diseño al equipo
- 🔍 Identificar problemas de diseño temprano

---

## Diagramas UML Más Útiles para Este Proyecto

### 1. Diagrama de Casos de Uso
Muestra QUÉ hace el sistema desde la perspectiva del usuario.

```
┌─────────────────────────────────────────┐
│         SISTEMA                         │
│                                         │
│    ┌─────────────────┐                  │
│    │  Registrar      │                  │
│    │  Usuario        │                  │
│    └─────────────────┘                  │
│           △                             │
│           │                             │
│    ┌──────┴──────┐                      │
│    │             │                      │
│ [Usuario]    [Administrador]            │
│                                         │
└─────────────────────────────────────────┘
```

### 2. Diagrama de Clases
Muestra la ESTRUCTURA de datos y sus relaciones.

```
┌─────────────────────┐       ┌─────────────────────┐
│      Usuario        │       │      Producto       │
├─────────────────────┤       ├─────────────────────┤
│ - id: int           │       │ - id: int           │
│ - nombre: string    │       │ - nombre: string    │
│ - email: string     │       │ - precio: float     │
│ - password: hash    │       │ - stock: int        │
├─────────────────────┤       ├─────────────────────┤
│ + login()           │       │ + actualizarStock() │
│ + registrar()       │       │ + getPrecio()       │
│ + actualizarPerfil()│       │                     │
└─────────────────────┘       └─────────────────────┘
         │                            │
         │           1                │      *
         │────────────────────────────│
                    compra
```

### 3. Diagrama de Secuencia
Muestra CÓMO interactúan los componentes en el tiempo.

```
 Usuario     →  Frontend   →   Backend   →   Base de Datos
    │              │             │               │
    │──Login────→  │             │               │
    │              │──POST /auth─→│               │
    │              │             │──Query───────→ │
    │              │             │               │
    │              │             │←─Datos───────  │
    │              │←─Token─────│               │
    │←─Redirigir── │             │               │
```

---

## Estructura de la Clase

### 1. Mini-Clase: Introducción a UML (10 minutos)
- Explicar los 3 tipos de diagramas
- Mostrar ejemplos aplicados

### 2. Taller Práctico (35 minutos)

**Herramienta recomendada:** [draw.io](https://app.diagrams.net/) (gratis, sin login)

**Parte 1: Casos de Uso (10 min)**
- Identifiquen los actores (usuarios, admin, etc.)
- Listen las acciones principales que puede hacer cada uno
- Dibujen el diagrama

**Parte 2: Clases Principal (15 min)**
- Identifiquen las entidades principales (Usuario, Producto, etc.)
- Para cada clase, definan:
  - Atributos (datos que guarda)
  - Métodos (acciones que puede hacer)
- Dibujen las relaciones (1 a muchos, muchos a muchos)

**Parte 3: Secuencia de una Acción (10 min)**
- Elijan UNA acción principal (ej: "comprar producto")
- Dibujen el flujo desde que el usuario hace clic hasta que se guarda en la BD

### 3. Cierre y Guardado (5 minutos)
- Exportar diagramas como PNG o PDF
- Guardar en: `grado_11/grupo_[nombre]/uml_clase6.drawio` (y exportar como PNG)

---

## Entregable

- **Archivos:**
  - `grado_11/grupo_[nombre]/uml_clase6.drawio` (archivo editable)
  - `grado_11/grupo_[nombre]/uml_clase6.png` (exportado para visualizar)
- Contenido:
  1. Diagrama de Casos de Uso
  2. Diagrama de Clases (al menos 3-4 clases principales)
  3. Diagrama de Secuencia (1 flujo principal)

---

## Rúbrica

| Criterio | Excelente (5) | Bueno (4) | Regular (3) |
|----------|---------------|-----------|-------------|
| Casos de uso | Todos los actores y acciones | Faltan 1-2 acciones | Incompleto |
| Clases | 4+ clases bien modeladas | 2-3 clases | 1 clase o mal modeladas |
| Secuencia | Flujo completo y lógico | Faltan pasos | Confuso |
| Notación UML | Símbolos correctos | Algunos errores | Errores graves |

---

## Plantilla para Empezar

```markdown
# DIAGRAMAS UML: [Nombre del Proyecto]

## Actores del Sistema
1. [Actor 1]: [rol/descripción]
2. [Actor 2]: [rol/descripción]

## Casos de Uso por Actor

### [Actor 1]
- [Caso de uso 1]
- [Caso de uso 2]
- [Caso de uso 3]

### [Actor 2]
- [Caso de uso 1]
- [Caso de uso 2]

## Clases Principales

### Clase 1: [Nombre]
**Atributos:**
- [atributo 1]: [tipo]
- [atributo 2]: [tipo]

**Métodos:**
- [método 1](): [qué hace]
- [método 2](): [qué hace]

### Clase 2: [Nombre]
[...]

## Relaciones
- [Clase 1] --(relación)--> [Clase 2]
- [Clase 3] --(hereda de)--> [Clase 4]

## Flujo Principal para Diagrama de Secuencia
[Describir paso a paso qué ocurre cuando el usuario hace X]
```

---

## Recursos

- [draw.io](https://app.diagrams.net/) - Herramienta gratuita de diagramas
- [UML Basics](https://www.uml.org/) - Documentación oficial
- [Lucidchart UML](https://www.lucidchart.com/pages/uml-class-diagram) - Tutoriales y ejemplos
