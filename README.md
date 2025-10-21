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

### 📁 Organización de Contenido

El repositorio está organizado en dos carpetas principales:

- **`/TS`** - Proyectos TypeScript ([Ver README](./TS))
- **`/Angular`** - Proyectos Angular ([Ver README](./Angular))

### 🚀 Proyectos TypeScript

<table>
<tr>
<td width="50%">

#### 📝 **Primer TypeScript**
📁 `/TS/PrimerTS`

Proyecto introductorio a TypeScript:
- Conceptos básicos de TypeScript
- Configuración inicial
- Compilación y ejecución
- Event handling básico

**Tecnologías:** TypeScript, lite-server

[📖 Ver README](./TS/PrimerTS)

</td>
<td width="50%">

#### 🧮 **Ejercicios TypeScript**
📁 `/TS/proy1`

Proyecto con ejercicios prácticos:
- Variables y tipos de datos
- Funciones y arrays
- Enums y matrices
- Operadores y control de flujo
- Tipos `any`, `unknown`, `void`, `never`

**Tecnologías:** TypeScript

[📖 Ver README](./TS/proy1)

</td>
</tr>
<tr>
<td width="50%">

#### 🔢 **Calculadora TypeScript**
📁 `/TS/calc`

Calculadora web con doble configuración:
- Implementación con **TypeScript**
- Dos variantes: lite-server y Vite
- Uso de **RxJS** para eventos
- Depuración con VSCode
- Sistema de operaciones básicas

**Tecnologías:** TypeScript, RxJS, Vite, HTML/CSS

[📖 Ver README](./TS/calc)

</td>
<td width="50%">

#### 📚 **Calculadora Ejemplo**
📁 `/TS/calc_ejemplo`

Versión de ejemplo de la calculadora:
- Implementación educativa
- Servidor con lite-server
- Ejercicios guiados

**Tecnologías:** TypeScript, lite-server

[📖 Ver README](./TS/calc_ejemplo)

</td>
</tr>
</table>

### 🅰️ Proyectos Angular

<table>
<tr>
<td width="50%">

#### 📱 **Proyecto1**
📁 `/Angular/Proyecto1`

Proyecto Angular básico:
- Generado con Angular CLI
- Arquitectura de componentes
- Desarrollo moderno con Angular 19

**Tecnologías:** Angular, TypeScript

[📖 Ver README](./Angular/Proyecto1)

</td>
</tr>
</table>

### 🔗 Submódulos (Repositorios Externos)

Este repositorio incluye referencias a proyectos más complejos que se mantienen en repositorios independientes:

#### TypeScript
- **[Calculadora-TS](https://github.com/Mariogarluu/Calculadora-TS)** 📁 `/TS/Calculadora` - Calculadora avanzada TypeScript
- **[api-db](https://github.com/Mariogarluu/api-db)** 📁 `/TS/api-db` - API Dragon Ball con TypeScript
- **[Api_Naruto](https://github.com/Mariogarluu/Api_Naruto)** 📁 `/TS/Api_Naruto` - API Naruto con TypeScript

#### Angular
- **[About_me Angular](https://github.com/Mariogarluu/Abouut_me_Angular)** 📁 `/Angular/About_me` - Página personal con Angular

> **Nota:** Los submódulos son repositorios independientes. Para clonarlos, usa:
> ```bash
> git submodule update --init --recursive
> ```

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

# 2. (Opcional) Clonar submódulos
git submodule update --init --recursive

# 3. Navegar al proyecto deseado
cd TS/PrimerTS  # o TS/calc, TS/proy1, Angular/Proyecto1, etc.

# 4. Instalar dependencias
npm install

# 5. Ejecutar en modo desarrollo
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

1. **`/TS/PrimerTS`** - Introducción a TypeScript
2. **`/TS/proy1`** - Ejercicios de tipos y sintaxis
3. **`/TS/calc`** - Aplicación práctica con eventos
4. **`/TS/Calculadora`** (submódulo) - Calculadora avanzada
5. **`/Angular/Proyecto1`** - Introducción a Angular
6. **Submódulos de APIs** - Proyectos completos con arquitectura avanzada

### Trabajar con Proyectos TypeScript

Ejemplo con PrimerTS:

```bash
cd TS/PrimerTS
npm install
npm start
```

### Trabajar con Calculadora

Proyecto educativo con dos configuraciones:

```bash
cd TS/calc
npm install
npm run dev
```

Incluye:
- ✅ Operaciones matemáticas básicas
- ✅ Manejo de errores
- ✅ Depuración con VSCode
- ✅ RxJS para eventos

### Trabajar con Submódulos

Para trabajar con los proyectos avanzados (submódulos):

```bash
# Inicializar y clonar submódulos
git submodule update --init --recursive

# Navegar al submódulo deseado
cd TS/api-db  # o TS/Api_Naruto, TS/Calculadora, Angular/About_me

# Consultar el README del submódulo para instrucciones específicas
cat README.md
```

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
