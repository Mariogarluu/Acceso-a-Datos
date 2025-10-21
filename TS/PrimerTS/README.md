# 📝 PrimerTS - Primer Proyecto TypeScript

Proyecto introductorio a TypeScript desarrollado para la asignatura de Acceso a Datos.

## 📋 Descripción

Este proyecto contiene los conceptos fundamentales de TypeScript, incluyendo configuración inicial, compilación y manejo básico de eventos. Es el punto de partida ideal para aprender TypeScript.

## 🎯 Objetivos de Aprendizaje

- ✅ Entender la configuración de TypeScript (tsconfig.json)
- ✅ Compilar código TypeScript a JavaScript
- ✅ Trabajar con tipos estáticos
- ✅ Manejar eventos del DOM con TypeScript
- ✅ Usar lite-server para desarrollo

## 🛠️ Tecnologías

- **TypeScript** - Lenguaje principal con tipado estático
- **lite-server** - Servidor de desarrollo ligero con live reload
- **HTML/CSS** - Estructura y estilos básicos

## 📂 Estructura del Proyecto

```
PrimerTS/
├── src/
│   ├── index.html         # Página principal
│   ├── index.ts           # Código TypeScript principal
│   └── styles.css         # Estilos (si aplica)
├── dist/                  # Código JavaScript compilado
├── node_modules/          # Dependencias
├── bs-config.json         # Configuración de lite-server
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
cd TS/PrimerTS

# 2. Instalar dependencias
npm install

# 3. Iniciar servidor de desarrollo
npm start
```

El navegador se abrirá automáticamente en `http://localhost:3000`

## 📜 Scripts Disponibles

```bash
npm start       # Inicia lite-server y abre el navegador
npm run compile # Compila TypeScript a JavaScript manualmente
```

## 🎓 Conceptos Implementados

### Tipos Básicos
```typescript
let nombre: string = "Mario";
let edad: number = 25;
let esEstudiante: boolean = true;
```

### Funciones con Tipado
```typescript
function saludar(nombre: string): string {
    return `Hola, ${nombre}!`;
}
```

### Manejo de Eventos
```typescript
const boton = document.getElementById('miBoton');
boton?.addEventListener('click', (event: Event) => {
    console.log('Botón clickeado');
});
```

### Configuración TypeScript
```json
{
  "compilerOptions": {
    "target": "ES6",
    "module": "commonjs",
    "outDir": "./dist",
    "rootDir": "./src",
    "strict": true
  }
}
```

## 📚 Contenido del Proyecto

1. **Configuración Inicial**
   - Instalación de TypeScript
   - Configuración de tsconfig.json
   - Setup de lite-server

2. **Tipos de Datos**
   - Tipos primitivos (string, number, boolean)
   - Arrays y tuplas
   - Tipos de unión

3. **Funciones**
   - Parámetros tipados
   - Valores de retorno tipados
   - Funciones flecha

4. **DOM Manipulation**
   - Selección de elementos
   - Event listeners
   - Type assertions

## 🔧 Configuración

### tsconfig.json

Archivo de configuración de TypeScript que define cómo se compila el código:

- **target**: ES6 - Versión de JavaScript de salida
- **module**: commonjs - Sistema de módulos
- **outDir**: ./dist - Carpeta de salida
- **rootDir**: ./src - Carpeta de código fuente
- **strict**: true - Modo estricto activado

### bs-config.json

Configuración de lite-server para desarrollo:

```json
{
  "server": {
    "baseDir": "./src"
  }
}
```

## 💡 Notas de Desarrollo

### Compilación Automática

El servidor lite-server no compila TypeScript automáticamente. Para desarrollo activo:

1. Opción 1: Compilar manualmente cuando haces cambios
2. Opción 2: Usar un watcher de TypeScript en otra terminal:
   ```bash
   tsc --watch
   ```

### Depuración

- Usa `console.log()` para debugging básico
- Los Source Maps están habilitados en tsconfig.json
- Puedes depurar directamente en el navegador

## 🐛 Solución de Problemas

### Error: "Cannot find module"
```bash
# Reinstalar dependencias
rm -rf node_modules package-lock.json
npm install
```

### TypeScript no compila
```bash
# Verificar configuración
cat tsconfig.json

# Compilar manualmente
npx tsc
```

### Puerto en uso
```bash
# lite-server usa el puerto 3000 por defecto
# Si está ocupado, cierra la aplicación que lo usa o modifica bs-config.json
```

## 📚 Recursos Adicionales

- [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)
- [TypeScript Playground](https://www.typescriptlang.org/play)
- [lite-server Documentation](https://github.com/johnpapa/lite-server)

## 🎯 Próximos Pasos

Después de completar este proyecto, continúa con:
1. **proy1** - Ejercicios más avanzados de TypeScript
2. **calc** - Aplicación práctica con RxJS
3. **Submódulos** - Proyectos completos y avanzados

---

[⬅️ Volver a Proyectos TypeScript](../README.md) | [⬅️ Volver al README principal](../../README.md)
