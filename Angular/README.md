# 🅰️ Proyectos Angular

Esta carpeta contiene los proyectos desarrollados con Angular para la asignatura de Acceso a Datos.

## 📂 Estructura de Proyectos

### 🎓 Proyectos de Aprendizaje

#### 📱 Proyecto1
**Descripción:** Proyecto básico de Angular  
**Ubicación:** `/Angular/Proyecto1`  
**Nivel:** Principiante  
**Versión Angular:** 19.2.18

Contenido:
- Estructura básica de proyecto Angular
- Componentes y arquitectura modular
- Routing y navegación
- Generado con Angular CLI
- Configuración de desarrollo moderno

**Tecnologías:** Angular 19, TypeScript, Angular CLI

**Iniciar proyecto:**
```bash
cd Proyecto1
npm install
ng serve
```

Accede a la aplicación en `http://localhost:4200/`

[📖 Ver README detallado](./Proyecto1/README.md)

---

## 🔗 Submódulos (Proyectos Avanzados)

Los siguientes son repositorios independientes incluidos como submódulos. Cada uno es un proyecto completo con su propia documentación.

### 👤 About_me Angular
**Repositorio:** [Mariogarluu/Abouut_me_Angular](https://github.com/Mariogarluu/Abouut_me_Angular)  
**Ubicación:** `/Angular/About_me`  
**Nivel:** Intermedio-Avanzado  

Página personal desarrollada con Angular. Incluye características avanzadas y diseño moderno. Consulta el repositorio original para más detalles sobre funcionalidades, configuración e instalación.

**Inicializar submódulo:**
```bash
git submodule update --init Angular/About_me
cd About_me
# Consultar README del submódulo para instrucciones específicas
```

---

## 🚀 Inicio Rápido

### Prerrequisitos

```bash
# Node.js (v18 o superior recomendado para Angular 19)
node --version

# npm (incluido con Node.js)
npm --version

# Angular CLI (instalación global)
npm install -g @angular/cli
```

### Clonar e Iniciar

```bash
# 1. Clonar el repositorio principal (si no lo has hecho)
git clone https://github.com/Mariogarluu/Acceso-a-Datos.git
cd Acceso-a-Datos/Angular

# 2. (Opcional) Inicializar submódulos
git submodule update --init --recursive

# 3. Elegir un proyecto e iniciar
cd Proyecto1
npm install
ng serve
```

## 📊 Comparación de Proyectos

| Proyecto | Nivel | Angular Version | Características |
|----------|-------|-----------------|-----------------|
| Proyecto1 | Principiante | 19.2.18 | Estructura básica, componentes |
| About_me (submódulo) | Intermedio-Avanzado | Ver repositorio | Página personal completa |

## 🎯 Ruta de Aprendizaje Recomendada

```
1. Proyecto1         → Fundamentos de Angular
2. About_me          → Proyecto completo y avanzado
```

## 🛠️ Scripts Comunes de Angular

Todos los proyectos Angular comparten estos scripts:

```bash
npm install          # Instalar dependencias
ng serve             # Servidor de desarrollo (http://localhost:4200)
ng build             # Compilar para producción
ng test              # Ejecutar tests unitarios
ng e2e               # Ejecutar tests end-to-end
ng generate          # Generar componentes, servicios, etc.
```

## 📚 Angular CLI - Comandos Útiles

### Generar Componentes
```bash
ng generate component nombre-componente
ng g c nombre-componente  # Forma corta
```

### Generar Servicios
```bash
ng generate service nombre-servicio
ng g s nombre-servicio  # Forma corta
```

### Generar Módulos
```bash
ng generate module nombre-modulo
ng g m nombre-modulo  # Forma corta
```

### Ver Ayuda
```bash
ng generate --help
ng --help
```

## 🏗️ Estructura Típica de Proyecto Angular

```
proyecto-angular/
├── src/
│   ├── app/                  # Componentes de la aplicación
│   │   ├── app.component.ts  # Componente raíz
│   │   ├── app.component.html
│   │   ├── app.component.css
│   │   └── app.config.ts     # Configuración de la app
│   ├── index.html            # Página principal
│   ├── main.ts               # Punto de entrada
│   └── styles.css            # Estilos globales
├── public/                   # Recursos estáticos
├── angular.json              # Configuración Angular CLI
├── package.json              # Dependencias
├── tsconfig.json             # Configuración TypeScript
└── README.md                 # Documentación
```

## 🎓 Conceptos Angular Clave

### Componentes
- Bloques de construcción de la aplicación
- Encapsulan vista, lógica y estilos
- Reutilizables y modulares

### Servicios
- Lógica de negocio compartida
- Inyección de dependencias
- Singleton por defecto

### Directivas
- Manipulación del DOM
- Directivas estructurales (*ngIf, *ngFor)
- Directivas de atributo

### Routing
- Navegación entre vistas
- Lazy loading de módulos
- Guards y resolvers

### Módulos
- Organización del código
- Encapsulación de funcionalidad
- Importación y exportación

## 📚 Recursos de Angular

### Documentación Oficial
- [Angular Documentation](https://angular.dev/)
- [Angular CLI Overview](https://angular.dev/tools/cli)
- [Angular Style Guide](https://angular.dev/style-guide)

### Tutoriales Recomendados
- [Tour of Heroes Tutorial](https://angular.dev/tutorial/tour-of-heroes)
- [Angular Getting Started](https://angular.dev/tutorials/first-app)

### Comunidad
- [Angular Blog](https://blog.angular.dev/)
- [Angular GitHub](https://github.com/angular/angular)

## 🔧 Solución de Problemas Comunes

### Error al servir el proyecto
```bash
# Limpiar caché y reinstalar
rm -rf node_modules package-lock.json
npm install
```

### Puerto 4200 en uso
```bash
# Usar un puerto diferente
ng serve --port 4201
```

### Actualizar Angular CLI
```bash
npm uninstall -g @angular/cli
npm install -g @angular/cli@latest
```

---

[⬅️ Volver al README principal](../README.md)
