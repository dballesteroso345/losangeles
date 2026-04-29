# Clase 4 - Grado 11: Arquitectura del Sistema

**Duración:** 50 minutos  
**Sala:** Sala de sistemas  
**Objetivo:** Definir la arquitectura técnica del proyecto de grado

---

## Contexto

Están en la **Semana 5-6: Diseño de Solución**. Ya validaron su problema y definieron qué van a construir. Ahora necesitan planificar **CÓMO** lo van a construir técnicamente.

---

## ¿Qué es la Arquitectura de Software?

Es la **estructura fundamental** de tu sistema. Define:
- 🏗️ Cómo se organizan los componentes
- 🔌 Cómo se comunican entre sí
- 📦 Qué tecnologías usarás
- 🔄 Cómo fluyen los datos

**¿Por qué importa?** Una buena arquitectura hace que el proyecto sea:
- ✅ Más fácil de desarrollar
- ✅ Más fácil de mantener
- ✅ Más escalable (puede crecer)
- ✅ Menos propenso a bugs

---

## Componentes de una Arquitectura Típica

### Para Aplicación Web (Full-Stack)

```
┌─────────────────────────────────────────────────┐
│                    CLIENTE                      │
│  ┌─────────────────────────────────────────┐    │
│  │           Frontend (React/Vue)          │    │
│  │  - Interfaz de usuario                  │    │
│  │  - Lógica de presentación               │    │
│  │  - Consumo de API                       │    │
│  └─────────────────────────────────────────┘    │
│                      │                          │
│                      │ HTTP/REST                │
│                      ▼                          │
│  ┌─────────────────────────────────────────┐    │
│  │            Backend (Node.js)            │    │
│  │  - API endpoints                        │    │
│  │  - Lógica de negocio                    │    │
│  │  - Autenticación                        │    │
│  └─────────────────────────────────────────┘    │
│                      │                          │
│                      │ SQL                      │
│                      ▼                          │
│  ┌─────────────────────────────────────────┐    │
│  │        Base de Datos (PostgreSQL)       │    │
│  │  - Tablas de usuarios                   │    │
│  │  - Datos del dominio                    │    │
│  └─────────────────────────────────────────┘    │
└─────────────────────────────────────────────────┘
```

### Para Aplicación de Escritorio/Móvil

```
┌─────────────────────────────────────────────────┐
│              APLICACIÓN (Flutter/React Native)  │
│  ┌─────────────────────────────────────────┐    │
│  │           Capa de Presentación          │    │
│  │  - Pantallas/Vistas                     │    │
│  │  - Componentes UI                       │    │
│  └─────────────────────────────────────────┘    │
│                      │                          │
│                      ▼                          │
│  ┌─────────────────────────────────────────┐    │
│  │           Capa de Lógica                │    │
│  │  - Servicios                            │    │
│  │  - Modelos de dominio                   │    │
│  │  - Validaciones                         │    │
│  └─────────────────────────────────────────┘    │
│                      │                          │
│                      ▼                          │
│  ┌─────────────────────────────────────────┐    │
│  │         Capa de Datos                   │    │
│  │  - API local/remota                     │    │
│  │  - Almacenamiento local                 │    │
│  └─────────────────────────────────────────┘    │
└─────────────────────────────────────────────────┘
```

### Para Proyecto de IA/Data Science

```
┌─────────────────────────────────────────────────┐
│           SISTEMA DE IA                         │
│  ┌─────────────────────────────────────────┐    │
│  │         Interfaz (Streamlit/Web)        │    │
│  │  - Input del usuario                    │    │
│  │  - Visualización de resultados          │    │
│  └─────────────────────────────────────────┘    │
│                      │                          │
│                      ▼                          │
│  ┌─────────────────────────────────────────┐    │
│  │        Pipeline de IA                   │    │
│  │  - Preprocesamiento                     │    │
│  │  - Modelo (TensorFlow/PyTorch)          │    │
│  │  - Postprocesamiento                    │    │
│  └─────────────────────────────────────────┘    │
│                      │                          │
│                      ▼                          │
│  ┌─────────────────────────────────────────┐    │
│  │           Datos                         │    │
│  │  - Dataset de entrenamiento             │    │
│  │  - Datos de entrada                     │    │
│  └─────────────────────────────────────────┘    │
└─────────────────────────────────────────────────┘
```

---

## Estructura de la Clase

### 1. Mini-Clase: Conceptos de Arquitectura (15 minutos)
- Patrones comunes (MVC, Capas, Cliente-Servidor)
- Cómo elegir la arquitectura correcta para TU proyecto

### 2. Taller: Definir TU Arquitectura (25 minutos)

Completen este documento:

```markdown
# ARQUITECTURA DEL SISTEMA

## Proyecto: [Nombre del Proyecto]

## 1. Tipo de Aplicación
[ ] Web (Frontend + Backend + BD)
[ ] Móvil (iOS/Android)
[ ] Escritorio
[ ] IA/ML
[ ] Automatización
[ ] Otro: _______

## 2. Diagrama de Arquitectura
[Dibujen o describan cómo se conectan los componentes]

## 3. Componentes Principales

### Componente 1: [Nombre]
- **Responsabilidad:** ¿Qué hace?
- **Tecnología:** ¿Con qué?
- **Entradas:** ¿Qué recibe?
- **Salidas:** ¿Qué produce?

### Componente 2: [Nombre]
- **Responsabilidad:**
- **Tecnología:**
- **Entradas:**
- **Salidas:**

### Componente 3: [Nombre]
- **Responsabilidad:**
- **Tecnología:**
- **Entradas:**
- **Salidas:**

## 4. Flujo de Datos
[Describan cómo viaja un dato desde que el usuario interactúa hasta que se guarda/muestra]

## 5. Decisiones Arquitectónicas
- ¿Por qué eligieron esta arquitectura?
- ¿Qué alternativas consideraron?
- ¿Qué trade-offs (ventajas/desventajas) aceptaron?
```

### 3. Cierre (10 minutos)
- 2-3 grupos comparten su arquitectura
- Feedback del profesor y compañeros

---

## Entregable

- **Archivo:** `grado_11/grupo_[nombre]/arquitectura_clase4.md`
- Documento de arquitectura completo con diagrama

---

## Rúbrica

| Criterio | Excelente (5) | Bueno (4) | Regular (3) |
|----------|---------------|-----------|-------------|
| Claridad | Arquitectura fácil de entender | Comprensible | Confusa |
| Componentes | Bien definidos y separados | Definidos | Solapados o vagos |
| Tecnologías | Adecuadas al problema | Aceptables | No claras o inadecuadas |
| Justificación | Decisiones bien razonadas | Algo razonadas | Sin justificación |

---

## Recursos

- [Patrones de Arquitectura](https://refactoring.guru/es/design-patterns)
- [System Design Primer](https://github.com/donnemartin/system-design-primer)
