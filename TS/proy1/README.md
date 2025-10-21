# 🧮 proy1 - Ejercicios TypeScript

Colección de ejercicios prácticos para aprender TypeScript desarrollados para la asignatura de Acceso a Datos.

## 📋 Descripción

Este proyecto contiene una serie de ejercicios diseñados para practicar los conceptos fundamentales y avanzados de TypeScript, incluyendo tipos de datos, funciones, arrays, enums, matrices y tipos especiales.

## 🎯 Objetivos de Aprendizaje

- ✅ Dominar tipos de datos en TypeScript
- ✅ Trabajar con funciones tipadas
- ✅ Manipular arrays y estructuras de datos
- ✅ Usar enums y tipos especiales
- ✅ Entender matrices y operaciones
- ✅ Aplicar operadores y control de flujo
- ✅ Comprender tipos `any`, `unknown`, `void`, `never`

## 🛠️ Tecnologías

- **TypeScript** - Lenguaje principal con tipado estático
- **Node.js** - Entorno de ejecución
- **npm** - Gestor de paquetes

## 📂 Estructura del Proyecto

```
proy1/
├── src/
│   ├── ejercicio1.ts      # Variables y tipos básicos
│   ├── ejercicio2.ts      # Funciones y métodos
│   ├── ejercicio3.ts      # Arrays y manipulación
│   ├── ejercicio4.ts      # Enums y tipos especiales
│   ├── ejercicio5.ts      # Matrices
│   └── ...                # Más ejercicios
├── dist/                  # Código JavaScript compilado
├── node_modules/          # Dependencias
├── .vscode/               # Configuración de VSCode
├── Calculadora/           # Proyecto adicional
├── tsconfig.json          # Configuración de TypeScript
├── package.json           # Dependencias del proyecto
└── README.md              # Este archivo
```

## 🚀 Inicio Rápido

### Prerrequisitos

```bash
node --version  # v14 o superior
npm --version
```

### Instalación

```bash
# 1. Navegar al proyecto
cd TS/proy1

# 2. Instalar dependencias
npm install

# 3. Compilar TypeScript
npm run build
# o
npx tsc

# 4. Ejecutar un ejercicio específico
node dist/ejercicio1.js
```

## 📜 Scripts Disponibles

```bash
npm install     # Instalar dependencias
npm run build   # Compilar TypeScript a JavaScript
npm start       # Compilar y ejecutar (si está configurado)
npx tsc         # Compilar manualmente con TypeScript
```

## 🎓 Ejercicios Incluidos

### 1. Variables y Tipos de Datos
Conceptos cubiertos:
- Tipos primitivos: `string`, `number`, `boolean`
- Arrays y tuplas
- Objetos y tipos personalizados
- Type inference
- Type annotations

### 2. Funciones
Conceptos cubiertos:
- Parámetros tipados
- Tipos de retorno
- Parámetros opcionales y por defecto
- Funciones flecha
- Sobrecarga de funciones

### 3. Arrays
Conceptos cubiertos:
- Declaración y tipado de arrays
- Métodos de arrays (map, filter, reduce)
- Arrays multidimensionales
- Iteración de arrays
- Desestructuración

### 4. Enums
Conceptos cubiertos:
- Enums numéricos
- Enums de cadena
- Enums heterogéneos
- Enums computados
- Uso práctico de enums

### 5. Matrices
Conceptos cubiertos:
- Arrays bidimensionales
- Recorrido de matrices
- Operaciones con matrices
- Transformaciones

### 6. Operadores y Control de Flujo
Conceptos cubiertos:
- Operadores aritméticos
- Operadores lógicos
- Operadores de comparación
- if/else, switch
- Bucles (for, while, do-while)

### 7. Tipos Especiales
Conceptos cubiertos:
- `any`: Tipo que desactiva el chequeo de tipos
- `unknown`: Versión segura de any
- `void`: Ausencia de tipo de retorno
- `never`: Tipo que nunca retorna
- `null` y `undefined`

## 💻 Ejemplos de Código

### Variables y Tipos
```typescript
// Tipos básicos
let nombre: string = "Mario";
let edad: number = 25;
let activo: boolean = true;

// Arrays
let numeros: number[] = [1, 2, 3, 4, 5];
let nombres: Array<string> = ["Ana", "Juan", "María"];

// Tuplas
let persona: [string, number] = ["Mario", 25];
```

### Funciones
```typescript
// Función con tipos
function sumar(a: number, b: number): number {
    return a + b;
}

// Función con parámetros opcionales
function saludar(nombre: string, apellido?: string): string {
    return apellido ? `Hola ${nombre} ${apellido}` : `Hola ${nombre}`;
}

// Función flecha
const multiplicar = (a: number, b: number): number => a * b;
```

### Enums
```typescript
enum DiaSemana {
    Lunes = 1,
    Martes,
    Miercoles,
    Jueves,
    Viernes,
    Sabado,
    Domingo
}

let dia: DiaSemana = DiaSemana.Lunes;
console.log(dia); // 1
```

### Tipos Especiales
```typescript
// any - evitar cuando sea posible
let variable: any = "texto";
variable = 123; // OK

// unknown - más seguro que any
let dato: unknown = "texto";
if (typeof dato === "string") {
    console.log(dato.toUpperCase()); // OK después de verificar
}

// void - funciones sin retorno
function logMensaje(mensaje: string): void {
    console.log(mensaje);
}

// never - funciones que nunca retornan
function error(mensaje: string): never {
    throw new Error(mensaje);
}
```

### Matrices
```typescript
// Matriz bidimensional
let matriz: number[][] = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

// Recorrer matriz
for (let i = 0; i < matriz.length; i++) {
    for (let j = 0; j < matriz[i].length; j++) {
        console.log(matriz[i][j]);
    }
}
```

## 🔧 Configuración TypeScript

### tsconfig.json

```json
{
  "compilerOptions": {
    "target": "ES6",
    "module": "commonjs",
    "outDir": "./dist",
    "rootDir": "./src",
    "strict": true,
    "esModuleInterop": true,
    "skipLibCheck": true
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules"]
}
```

## 🐛 Solución de Problemas

### Error de compilación
```bash
# Verificar configuración de TypeScript
cat tsconfig.json

# Limpiar dist y recompilar
rm -rf dist
npx tsc
```

### Tipos no reconocidos
```bash
# Reinstalar dependencias
npm install

# Verificar que @types/node está instalado (si usas Node.js APIs)
npm install --save-dev @types/node
```

## 📚 Recursos Adicionales

### Documentación
- [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)
- [TypeScript Deep Dive](https://basarat.gitbook.io/typescript/)
- [TypeScript Cheat Sheet](https://www.typescriptlang.org/cheatsheets)

### Herramientas
- [TypeScript Playground](https://www.typescriptlang.org/play)
- [TS Node](https://typestrong.org/ts-node/) - Ejecutar TypeScript directamente

### Práctica
- [TypeScript Exercises](https://typescript-exercises.github.io/)
- [Type Challenges](https://github.com/type-challenges/type-challenges)

## 🎯 Progresión Recomendada

1. **Variables y Tipos** → Fundamento esencial
2. **Funciones** → Bloques de construcción
3. **Arrays** → Estructuras de datos básicas
4. **Enums** → Valores constantes organizados
5. **Matrices** → Estructuras bidimensionales
6. **Operadores** → Lógica y control
7. **Tipos Especiales** → Casos avanzados

## 🎯 Próximos Pasos

Después de completar estos ejercicios, continúa con:
1. **calc** - Aplicación práctica con eventos y RxJS
2. **calc_ejemplo** - Implementación guiada de calculadora
3. **Submódulos** - Proyectos completos con APIs

---

[⬅️ Volver a Proyectos TypeScript](../README.md) | [⬅️ Volver al README principal](../../README.md)
