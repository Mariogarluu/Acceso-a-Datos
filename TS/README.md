# 📘 Proyectos TypeScript

Esta carpeta contiene todos los proyectos desarrollados con TypeScript para la asignatura de Acceso a Datos.

## 📂 Estructura de Proyectos

### 🎓 Proyectos de Aprendizaje

#### 📝 PrimerTS
**Descripción:** Proyecto introductorio a TypeScript  
**Ubicación:** `/TS/PrimerTS`  
**Nivel:** Principiante  

Contenido:
- Conceptos básicos de TypeScript
- Configuración inicial con tsconfig.json
- Compilación y ejecución con lite-server
- Event handling básico
- Primeros pasos con tipos estáticos

**Iniciar proyecto:**
```bash
cd PrimerTS
npm install
npm start
```

[📖 Ver README detallado](./PrimerTS/README.md)

---

#### 🧮 proy1
**Descripción:** Ejercicios prácticos de TypeScript  
**Ubicación:** `/TS/proy1`  
**Nivel:** Principiante-Intermedio  

Contenido:
- Variables y tipos de datos
- Funciones y métodos
- Arrays y manipulación de datos
- Enums y tipos especiales
- Matrices y estructuras de datos
- Operadores y control de flujo
- Tipos `any`, `unknown`, `void`, `never`

**Iniciar proyecto:**
```bash
cd proy1
npm install
npm start
```

[📖 Ver README detallado](./proy1/README.md)

---

#### 🔢 calc
**Descripción:** Calculadora web con TypeScript y RxJS  
**Ubicación:** `/TS/calc`  
**Nivel:** Intermedio  

Contenido:
- Implementación de calculadora funcional
- Dos configuraciones: lite-server y Vite
- Uso de RxJS para manejo de eventos
- Depuración con VSCode
- Operaciones matemáticas básicas
- Manejo de errores y validación

**Tecnologías:** TypeScript, RxJS, Vite, HTML/CSS

**Iniciar proyecto:**
```bash
cd calc
npm install
npm run dev  # Con Vite (recomendado)
```

[📖 Ver README detallado](./calc/README.md)

---

#### 📚 calc_ejemplo
**Descripción:** Versión de ejemplo de la calculadora  
**Ubicación:** `/TS/calc_ejemplo`  
**Nivel:** Principiante  

Contenido:
- Implementación educativa simplificada
- Servidor con lite-server
- Código comentado y documentado
- Ejercicios guiados

**Iniciar proyecto:**
```bash
cd calc_ejemplo
npm install
npm start
```

[📖 Ver README detallado](./calc_ejemplo/README.md)

---

## 🔗 Submódulos (Proyectos Avanzados)

Los siguientes son repositorios independientes incluidos como submódulos. Cada uno es un proyecto completo con su propia documentación.

### 🧮 Calculadora-TS
**Repositorio:** [Mariogarluu/Calculadora-TS](https://github.com/Mariogarluu/Calculadora-TS)  
**Ubicación:** `/TS/Calculadora`  
**Nivel:** Avanzado  

Calculadora avanzada con características extendidas. Consulta el repositorio original para más detalles.

**Inicializar submódulo:**
```bash
git submodule update --init TS/Calculadora
cd Calculadora
# Consultar README del submódulo para instrucciones específicas
```

---

### 🐉 api-db (Dragon Ball API)
**Repositorio:** [Mariogarluu/api-db](https://github.com/Mariogarluu/api-db)  
**Ubicación:** `/TS/api-db`  
**Nivel:** Avanzado  

Aplicación completa para consumo de API de Dragon Ball con arquitectura avanzada. Consulta el repositorio original para más detalles.

**Inicializar submódulo:**
```bash
git submodule update --init TS/api-db
cd api-db
# Consultar README del submódulo para instrucciones específicas
```

---

### 🍥 Api_Naruto
**Repositorio:** [Mariogarluu/Api_Naruto](https://github.com/Mariogarluu/Api_Naruto)  
**Ubicación:** `/TS/Api_Naruto`  
**Nivel:** Avanzado  

Aplicación para explorar el universo de Naruto mediante API. Consulta el repositorio original para más detalles.

**Inicializar submódulo:**
```bash
git submodule update --init TS/Api_Naruto
cd Api_Naruto
# Consultar README del submódulo para instrucciones específicas
```

---

## 🚀 Inicio Rápido

### Prerrequisitos
```bash
node --version  # v14 o superior
npm --version
```

### Clonar e Iniciar

```bash
# 1. Clonar el repositorio principal (si no lo has hecho)
git clone https://github.com/Mariogarluu/Acceso-a-Datos.git
cd Acceso-a-Datos/TS

# 2. (Opcional) Inicializar submódulos
git submodule update --init --recursive

# 3. Elegir un proyecto e iniciar
cd PrimerTS
npm install
npm start
```

## 📊 Comparación de Proyectos

| Proyecto | Nivel | Tecnologías Principales | Características |
|----------|-------|------------------------|-----------------|
| PrimerTS | Principiante | TypeScript, lite-server | Conceptos básicos |
| proy1 | Principiante-Intermedio | TypeScript | Ejercicios prácticos |
| calc_ejemplo | Principiante | TypeScript, lite-server | Calculadora simple |
| calc | Intermedio | TypeScript, RxJS, Vite | Calculadora con eventos reactivos |
| Calculadora (submódulo) | Avanzado | Ver repositorio | Calculadora avanzada |
| api-db (submódulo) | Avanzado | Ver repositorio | Consumo de API Dragon Ball |
| Api_Naruto (submódulo) | Avanzado | Ver repositorio | Consumo de API Naruto |

## 🎯 Ruta de Aprendizaje Recomendada

```
1. PrimerTS          → Fundamentos de TypeScript
2. proy1             → Práctica de tipos y sintaxis  
3. calc_ejemplo      → Aplicación simple
4. calc              → RxJS y programación reactiva
5. Submódulos        → Proyectos completos y avanzados
```

## 🛠️ Scripts Comunes

Todos los proyectos TypeScript comparten scripts similares:

```bash
npm install    # Instalar dependencias
npm start      # Iniciar servidor de desarrollo
npm run dev    # Alias para start (en proyectos con Vite)
npm run build  # Compilar TypeScript (cuando aplique)
```

## 📚 Recursos

- [TypeScript Handbook](https://www.typescriptlang.org/docs/)
- [RxJS Documentation](https://rxjs.dev/)
- [Vite Guide](https://vitejs.dev/guide/)

---

[⬅️ Volver al README principal](../README.md)