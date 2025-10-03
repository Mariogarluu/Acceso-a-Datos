<div align="center">

# 📚 Acceso a Datos - DAM

### *Repositorio de la asignatura Acceso a Datos*
### *Desarrollo de Aplicaciones Multiplataforma*

[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![RxJS](https://img.shields.io/badge/RxJS-B7178C?style=for-the-badge&logo=reactivex&logoColor=white)](https://rxjs.dev/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)

*Colección de proyectos y ejercicios desarrollados con TypeScript, RxJS y tecnologías web modernas*

</div>

---

## 📖 Descripción

Este repositorio contiene los proyectos y ejercicios desarrollados durante la asignatura de **Acceso a Datos** del ciclo formativo de Desarrollo de Aplicaciones Multiplataforma (DAM). Los proyectos están enfocados en el aprendizaje de TypeScript, programación reactiva con RxJS, y desarrollo web moderno.

## 🎯 Objetivos de Aprendizaje

- ✅ Dominio de **TypeScript** y tipado estático
- ✅ Programación reactiva con **RxJS**
- ✅ Arquitecturas modulares y escalables
- ✅ Desarrollo web moderno con **Vite**
- ✅ Consumo de APIs y manejo de datos
- ✅ Patrones de diseño y buenas prácticas

## 📂 Estructura del Repositorio

### 🚀 Proyectos Principales

<table>
<tr>
<td width="50%">

#### 🐉 **Dragon Ball Universe Explorer**
📁 `/dragon-ball-ux`

Aplicación web moderna para explorar el universo de Dragon Ball:
- **TypeScript** con arquitectura modular
- **RxJS** para programación reactiva
- **Tailwind CSS** para estilos modernos
- Consumo de API Dragon Ball
- Sistema de paginación y búsqueda
- Modales y componentes interactivos

**Tecnologías:** TypeScript, RxJS, Vite, Tailwind CSS

[📖 Ver README completo](./dragon-ball-ux/README.md)

</td>
<td width="50%">

#### 🔢 **Calculadora TypeScript**
📁 `/calc`

Calculadora web con doble configuración:
- Implementación con **TypeScript**
- Dos variantes: lite-server y Vite
- Uso de **RxJS** para eventos
- Depuración con VSCode
- Sistema de operaciones básicas

**Tecnologías:** TypeScript, RxJS, Vite, HTML/CSS

[📖 Ver README completo](./calc/README.md)

</td>
</tr>
<tr>
<td width="50%">

#### 📝 **Primer TypeScript**
📁 `/PrimerTS`

Proyecto introductorio a TypeScript:
- Conceptos básicos de TypeScript
- Configuración inicial
- Compilación y ejecución
- Event handling básico

**Tecnologías:** TypeScript, lite-server

</td>
<td width="50%">

#### 🧮 **Ejercicios TypeScript**
📁 `/proy1`

Proyecto con ejercicios prácticos:
- Variables y tipos de datos
- Funciones y arrays
- Enums y matrices
- Operadores y control de flujo
- Tipos `any`, `unknown`, `void`, `never`

**Tecnologías:** TypeScript

</td>
</tr>
</table>

### 📚 Proyectos de Ejemplo

- **`/calc_ejemplo`** - Versión de ejemplo de la calculadora
- **`/Calculadora`** - Directorio de recursos adicionales

## 🛠️ Tecnologías Utilizadas

### Lenguajes y Frameworks
- **TypeScript 5.x** - Lenguaje principal con tipado estático
- **JavaScript ES6+** - Compilación target
- **HTML5 & CSS3** - Estructura y estilos

### Librerías y Herramientas
- **RxJS 7.x** - Programación reactiva
- **Vite** - Build tool y dev server moderno
- **Tailwind CSS** - Framework de utilidades CSS
- **lite-server** - Servidor de desarrollo ligero

### Desarrollo
- **Node.js & npm** - Gestión de dependencias
- **VSCode** - Editor con configuración de debug
- **Git** - Control de versiones

## 🚀 Inicio Rápido

### Prerrequisitos

```bash
# Node.js (v14 o superior)
node --version

# npm (incluido con Node.js)
npm --version
```

### Instalación General

Cada proyecto tiene sus propias dependencias. Para instalar un proyecto específico:

```bash
# 1. Clonar el repositorio
git clone https://github.com/Mariogarluu/Acceso-a-Datos.git
cd Acceso-a-Datos

# 2. Navegar al proyecto deseado
cd dragon-ball-ux  # o calc, proy1, etc.

# 3. Instalar dependencias
npm install

# 4. Ejecutar en modo desarrollo
npm run dev
# o
npm start
```

### Scripts Comunes

La mayoría de proyectos comparten estos scripts:

| Script | Descripción |
|--------|-------------|
| `npm install` | Instalar dependencias |
| `npm run dev` | Servidor de desarrollo |
| `npm start` | Alias para dev |
| `npm run build` | Build para producción |
| `npm run preview` | Preview del build |

## 📋 Guía de Proyectos

### Proyecto Recomendado para Empezar

**Orden sugerido de aprendizaje:**

1. **`/PrimerTS`** - Introducción a TypeScript
2. **`/proy1`** - Ejercicios de tipos y sintaxis
3. **`/calc`** - Aplicación práctica con eventos
4. **`/dragon-ball-ux`** - Proyecto completo con arquitectura avanzada

### Dragon Ball Universe Explorer

El proyecto más completo del repositorio:

```bash
cd dragon-ball-ux
npm install
npm run dev
```

Características destacadas:
- 🎨 UI moderna con Tailwind CSS
- ⚡ Arquitectura modular con TypeScript
- 🔄 State management centralizado
- 🌐 Consumo de API externa
- 📱 Diseño responsive
- 🔍 Búsqueda y paginación

### Calculadora TypeScript

Proyecto educativo con dos configuraciones:

```bash
cd calc
npm install

# Opción 1: Con Vite (moderno)
npm run dev

# Opción 2: Con lite-server (clásico)
# Ver README del proyecto para más detalles
```

Incluye:
- ✅ Operaciones matemáticas básicas
- ✅ Manejo de errores
- ✅ Depuración con VSCode
- ✅ RxJS para eventos

## 🏗️ Arquitectura y Patrones

### Estructura de Proyecto Típica

```
proyecto/
├── src/
│   ├── index.ts          # Punto de entrada
│   ├── index.html        # Estructura HTML
│   ├── index.css         # Estilos
│   ├── types.ts          # Definiciones de tipos
│   ├── api.ts            # Servicios API
│   ├── managers/         # Gestores (State, UI)
│   └── modules/          # Módulos funcionales
├── dist/                 # Build de producción
├── package.json          # Dependencias
├── tsconfig.json         # Configuración TypeScript
├── vite.config.js        # Configuración Vite (si aplica)
└── README.md             # Documentación
```

### Patrones Utilizados

- **Módulos ES6** - Organización del código
- **Observables (RxJS)** - Programación reactiva
- **State Management** - Centralización del estado
- **Separation of Concerns** - Separación de responsabilidades
- **Type Safety** - Tipado fuerte con TypeScript

## 🎓 Conceptos Aprendidos

### TypeScript
- Tipos básicos y avanzados
- Interfaces y tipos personalizados
- Genéricos
- Decoradores
- Módulos y namespaces

### RxJS
- Observables y Subjects
- Operadores (map, filter, debounceTime, etc.)
- Subscripciones y gestión de memoria
- Programación reactiva funcional

### Desarrollo Web
- DOM manipulation
- Event handling
- Fetch API y HTTP
- Módulos ES6
- Build tools modernos

## 🤝 Contribución

Este es un repositorio educativo, pero las sugerencias son bienvenidas:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/MejorFeature`)
3. Commit tus cambios (`git commit -m 'Add: nueva característica'`)
4. Push a la rama (`git push origin feature/MejorFeature`)
5. Abre un Pull Request

## 📝 Recursos Adicionales

### Documentación Oficial
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)
- [RxJS Documentation](https://rxjs.dev/)
- [Vite Guide](https://vitejs.dev/guide/)
- [Tailwind CSS Docs](https://tailwindcss.com/docs)

### Tutoriales Recomendados
- [TypeScript para Principiantes](https://www.typescriptlang.org/docs/handbook/typescript-from-scratch.html)
- [RxJS Quick Start](https://rxjs.dev/guide/overview)
- [Modern JavaScript Tutorial](https://javascript.info/)

## 📄 Licencia

Este proyecto está desarrollado con fines educativos para la asignatura de Acceso a Datos.

**Uso libre para aprendizaje y referencia.**

---

<div align="center">

### 🌟 Desarrollado para DAM - Acceso a Datos 🌟

**Hecho con ❤️, TypeScript y RxJS**

[![TypeScript](https://img.shields.io/badge/TypeScript-Ready-blue.svg)](https://www.typescriptlang.org/)
[![Learning](https://img.shields.io/badge/Status-Learning-green.svg)](https://github.com/Mariogarluu/Acceso-a-Datos)

</div>
