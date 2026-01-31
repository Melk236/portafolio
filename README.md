# Portfolio README Interactivo

Portafolio de desarrollador con diseño de README.md de GitHub, implementado completamente en JavaScript Vanilla.

## 🚀 Características

### Diseño y Estética
- ✅ Apariencia exacta de README.md de GitHub
- ✅ Toggle modo claro/oscuro persistente
- ✅ Tipografía Markdown realista (Inter + JetBrains Mono)
- ✅ Syntax highlighting con Highlight.js
- ✅ Animaciones sutiles con CSS y JS
- ✅ 100% Responsive (mobile, tablet, desktop)

### Secciones Interactivas

#### 1. Header con Badges
- Badges de tecnologías interactivos
- Tooltips con nivel de experiencia y proyectos
- Clic para filtrar/focus
- Estadísticas de GitHub animadas

#### 2. Tabla de Contenidos
- Auto-generada desde los headings
- Scroll suave
- Indicador de sección activa
- Seguimiento de scroll en tiempo real

#### 3. About Me
- Biografía en formato Markdown
- Gráfico de contribuciones (heatmap) generado dinámicamente
- Gráfico de lenguajes más usados
- Código ejecutable en vivo

#### 4. Editor de Código
- Editor con textarea
- Botón Run para ejecutar JavaScript
- Output en tiempo real
- Botón Reset para restaurar código
- Syntax highlighting con Highlight.js

#### 5. Proyectos
- Lista de proyectos expandible (accordion)
- Screenshots con lightbox
- Badges de tecnologías
- Links a demo y repositorio

#### 6. Sistema de Commits
- Timeline de experiencia profesional
- Diseño tipo GitHub commits
- Cada trabajo es un "commit" en la carrera

#### 7. Skills
- Barras de progreso animadas
- Categorías: Frontend, Backend, Database, DevOps
- Animación al hacer scroll

#### 8. Contacto
- Tarjetas de contacto interactivas
- Botón copiar email al portapapeles
- Links a redes sociales
- Botón descargar CV

### Funcionalidades Interactivas

- **Búsqueda (Ctrl+K)**: Overlay de búsqueda con acciones rápidas
- **Autocompletado**: Sugerencias mientras escribes
- **Easter Egg**: Konami code (↑↑↓↓←→←→BA) activa mensaje secreto
- **Star Counter**: Botón para dar "stars" con contador animado
- **Raw Mode**: Ver el Markdown puro
- **Git Log**: Ver "commits" de la carrera en consola

## 🛠️ Tecnologías Utilizadas

- **HTML5** - Estructura semántica
- **Tailwind CSS** - Estilos utility-first
- **JavaScript Vanilla** - Lógica e interactividad
- **Lucide Icons** - Iconografía moderna
- **Highlight.js** - Syntax highlighting

## 📦 Dependencias Externas (CDN)

```html
<!-- Tailwind CSS -->
<script src="https://cdn.tailwindcss.com"></script>

<!-- Lucide Icons -->
<script src="https://unpkg.com/lucide@latest"></script>

<!-- Highlight.js -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/github.min.css">
<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js"></script>

<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
```

## 🚀 Cómo Usar

1. **Clona o descarga** este repositorio
2. **Abre** `index.html` en tu navegador
3. **Personaliza** los datos en la sección `DATA` del script
4. **Añade** tu foto de perfil como `moha.jpg`
5. **Añade** screenshots de proyectos

## 📝 Personalización

### Cambiar datos personales

Busca la sección `// ========== DATA ==========` en el script y modifica:

```javascript
const skills = {
    frontend: [
        { name: 'Tu Skill', level: 90, color: 'bg-red-500' },
        // ...
    ]
};

const personalData = {
    name: "Tu Nombre",
    role: "Tu Rol",
    // ...
};
```

### Agregar proyectos

Busca la sección de proyectos y añade nuevos collapsibles:

```html
<div class="collapsible" id="project-nuevo">
    <div class="collapsible-header" onclick="toggleCollapsible('project-nuevo')">
        <!-- Contenido -->
    </div>
    <div class="collapsible-content">
        <!-- Detalles -->
    </div>
</div>
```

### Cambiar temas

Los temas se manejan con variables CSS en `:root` y `.dark`. Puedes modificar los colores en la sección `<style>`.

## 🎨 Características Visuales

- **Typing Effect**: El título se escribe letra por letra
- **Fade In**: Las secciones aparecen con animación suave
- **Progress Bars**: Se animan al entrar en viewport
- **Heatmap**: Generado dinámicamente con colores de GitHub
- **Hover Effects**: En badges, botones y links

## ⌨️ Atajos de Teclado

| Atajo | Acción |
|-------|--------|
| `Ctrl + K` | Abrir búsqueda |
| `Esc` | Cerrar modales/búsqueda |
| `↑ ↑ ↓ ↓ ← → ← → B A` | Easter egg |

## 📱 Responsive

- **Desktop**: Layout completo con sidebar
- **Tablet**: Sidebar colapsable
- **Mobile**: Menú hamburguesa, layout vertical

## 🔧 Optimizaciones

- Intersection Observer para animaciones eficientes
- LocalStorage para persistir preferencias
- Lazy loading implícito con scroll
- Event delegation para mejor performance

## 🐛 Debugging

Abre la consola del navegador para ver:
- Git log de la carrera
- Mensajes de easter eggs
- Errores de ejecución de código

## 📄 Licencia

Este proyecto es de uso libre. Puedes usarlo como base para tu propio portafolio.

---

**Hecho con 💻 y ❤️ por Mohamed El Khassal**

⭐ Si te gustó este proyecto, ¡dale una star!
