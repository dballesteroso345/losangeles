# Clase 5 - Grado 11: Stack Tecnológico

**Duración:** 50 minutos  
**Sala:** Sala de sistemas  
**Objetivo:** Seleccionar las tecnologías específicas para construir el proyecto

---

## ¿Qué es el Stack Tecnológico?

El **stack** es el conjunto de lenguajes, frameworks, librerías y herramientas que usarán para construir su proyecto.

**Una buena elección de stack:**
- ✅ Acelera el desarrollo
- ✅ Tiene buena documentación
- ✅ Es escalable (puede crecer)
- ✅ Tiene comunidad activa

**Una mala elección:**
- ❌ Te hace reinventar la rueda
- ❌ No tiene tutoriales ni ayuda
- ❌ No escala con tu proyecto

---

## Stacks Comunes por Tipo de Proyecto

### 1. Aplicación Web Full-Stack

```
┌─────────────────────────────────────────┐
│           FRONTEND                      │
│  - React / Vue / Angular                │
│  - TypeScript (opcional)                │
│  - Tailwind / Material UI               │
└─────────────────────────────────────────┘
                    │
                    │ API REST / GraphQL
                    ▼
┌─────────────────────────────────────────┐
│           BACKEND                       │
│  - Node.js (Express, NestJS)            │
│  - Python (FastAPI, Django, Flask)      │
│  - Go (Gin, Echo)                       │
└─────────────────────────────────────────┘
                    │
                    │ SQL / NoSQL
                    ▼
┌─────────────────────────────────────────┐
│         BASE DE DATOS                   │
│  - PostgreSQL (relacional)              │
│  - MongoDB (documentos)                 │
│  - Firebase (BaaS)                      │
└─────────────────────────────────────────┘
```

**Stack recomendado para principiantes:**
- Frontend: React + Vite
- Backend: Node.js + Express
- BD: PostgreSQL o Firebase

### 2. Aplicación Móvil

```
┌─────────────────────────────────────────┐
│         MULTIPLATAFORMA                 │
│  - Flutter (Dart) → iOS + Android       │
│  - React Native (JavaScript)            │
└─────────────────────────────────────────┘
                    │
                    ▼
┌─────────────────────────────────────────┐
│         BACKEND / API                   │
│  - Firebase (autenticación + DB)        │
│  - API propia (Node, Python)            │
└─────────────────────────────────────────┘
```

**Stack recomendado:**
- Flutter + Firebase (más fácil)
- React Native + API propia (si ya saben React)

### 3. Proyecto de IA / Data Science

```
┌─────────────────────────────────────────┐
│         INTERFAZ                        │
│  - Streamlit (rápido)                   │
│  - Gradio (ML específico)               │
│  - Flask/FastAPI + frontend             │
└─────────────────────────────────────────┘
                    │
                    ▼
┌─────────────────────────────────────────┐
│         NÚCLEO DE IA                    │
│  - Python                               │
│  - TensorFlow / PyTorch                 │
│  - Scikit-learn                         │
│  - Pandas, NumPy                        │
└─────────────────────────────────────────┘
```

**Stack recomendado:**
- Python + Streamlit + scikit-learn/TensorFlow

### 4. Automatización / Scripts

```
┌─────────────────────────────────────────┐
│         SCRIPT / BOT                    │
│  - Python                               │
│  - Selenium (web automation)            │
│  - PyAutoGUI (GUI automation)           │
│  - APIs varias                          │
└─────────────────────────────────────────┘
```

---

## Estructura de la Clase

### 1. Presentación de Opciones (15 minutos)
- Revisar stacks por tipo de proyecto
- Discutir pros y contras de cada uno

### 2. Taller: Seleccionar SU Stack (25 minutos)

Completen esta plantilla:

```markdown
# STACK TECNOLÓGICO: [Nombre del Proyecto]

## Tipo de Proyecto
[ ] Web
[ ] Móvil
[ ] IA/ML
[ ] Automatización
[ ] Otro: _______

## Frontend / Interfaz

**Tecnología principal:**
[React/Vue/Flutter/Streamlit/etc.]

**Por qué la elegimos:**
[Razones]

**UI/Styling:**
[Tailwind/Material UI/etc.]

## Backend / Lógica

**Lenguaje:**
[Node.js/Python/Go/etc.]

**Framework:**
[Express/FastAPI/etc.]

**Por qué lo elegimos:**
[Razones]

## Base de Datos / Almacenamiento

**Tipo:**
[SQL/NoSQL/Archivos/Firebase]

**Tecnología específica:**
[PostgreSQL/MongoDB/Firebase/etc.]

**Por qué la elegimos:**
[Razones]

## Herramientas Adicionales

**Control de versiones:** Git + [GitHub/GitLab]

**Autenticación:**
[Propia/Firebase/Auth0/etc.]

**Deploy/Hosting:**
[Vercel/Netlify/Heroku/Railway/etc.]

## Decisiones Clave

1. [Decisión 1 + justificación]
2. [Decisión 2 + justificación]
3. [Decisión 3 + justificación]
```

### 3. Validación Técnica (10 minutos)
- Verificar que existan tutoriales para su stack
- Confirmar que las tecnologías son compatibles entre sí
- Identificar posibles obstáculos

---

## Entregable

- **Archivo:** `grado_11/grupo_[nombre]/stack_clase5.md`
- Documento de stack tecnológico completo con justificaciones

---

## Rúbrica

| Criterio | Excelente (5) | Bueno (4) | Regular (3) |
|----------|---------------|-----------|-------------|
| Completitud | Todas las capas definidas | Faltan 1-2 capas | Incompleto |
| Justificación | Cada elección bien razonada | Algunas razones | Sin justificar |
| Adecuación | Stack apropiado al proyecto | Aceptable | Inadecuado |
| Investigación | Menciona alternativas consideradas | Pocas alternativas | Sin investigación |

---

## Recursos

- [StackShare](https://stackshare.io/) - Ver qué stacks usan empresas reales
- [Roadmap.sh](https://roadmap.sh/) - Roadmaps de aprendizaje por tecnología
- [Firebase](https://firebase.google.com/) - Backend como servicio (fácil para prototipos)
- [Vercel](https://vercel.com/) - Hosting gratuito para frontend
- [Railway](https://railway.app/) - Hosting para backend + BD
