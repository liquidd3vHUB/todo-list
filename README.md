# 📋 To-Do List Avanzada

Una aplicación web moderna y completa para gestionar tareas personales con características avanzadas, interfaz intuitiva y soporte para modo oscuro.

## ✨ Características Principales

### Gestión de Tareas
- ✅ **Crear tareas** con título, descripción, categoría, prioridad y fecha de vencimiento
- 📝 **Editar tareas** (marcar como completadas, eliminar)
- 🗑️ **Eliminar tareas** individuales o en lote (eliminar todas las completadas)
- 🎯 **Marcar como completada** con interfaz interactiva
- 📂 **Categorización** de tareas con 5 categorías predeterminadas (Trabajo, Personal, Hogar, Salud, Otros)
- 🏷️ **Crear nuevas categorías** dinámicamente
- 🔴 **Niveles de prioridad**: Alta, Media, Baja

### Búsqueda y Filtrado
- 🔍 **Barra de búsqueda** en tiempo real (busca por título y descripción)
- 📊 **Filtros por estado**: Todas, Pendientes, Completadas
- 🎯 **Filtro por prioridad**: Ver tareas por nivel de prioridad
- 📁 **Filtro por categoría**: Hacer clic en una categoría para filtrar
- 🔗 **Filtros combinados**: Usar múltiples filtros simultáneamente

### Ordenamiento
- 📅 **Por fecha de vencimiento**: Tareas próximas a vencer primero
- 📌 **Por prioridad**: Tareas de alta prioridad primero
- 🕐 **Por fecha de creación**: Tareas más recientes primero

### Estadísticas y Monitoreo
- 📊 **Sidebar con estadísticas**:
  - Total de tareas
  - Tareas completadas
  - Tareas pendientes
- 📁 **Panel de categorías** con contador de tareas por categoría
- ⏰ **Indicadores visuales** de tareas vencidas

### Funcionalidades Avanzadas
- 🎨 **Modo oscuro/claro**: Toggle para cambiar tema
- 🖱️ **Drag and Drop**: Reordenar tareas arrastrando
- 💾 **Persistencia de datos**: LocalStorage para guardar automáticamente
- ⚠️ **Detección de tareas vencidas**: Resaltado visual de tareas por vencer
- 🎯 **Validación de formularios**: Campos requeridos y validación básica
- 🛡️ **Protección contra inyecciones**: Escapado de HTML para seguridad
- ♿ **Accesibilidad**: Etiquetas ARIA y roles semánticos

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Estilos avanzados con:
  - CSS Variables para temas
  - Flexbox y Grid para layouts responsivos
  - Transiciones y animaciones fluidas
  - Modo oscuro con variables dinámicas
- **JavaScript Vanilla**: Lógica sin dependencias externas
  - Programación orientada a objetos (Clase `TodoApp`)
  - Manipulación del DOM
  - Event listeners y delegación de eventos
  - LocalStorage API

## 🚀 Instalación y Uso

### Requisitos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- No requiere instalación de dependencias

### Pasos para usar

1. **Descargar o clonar** el proyecto
2. **Abrir el archivo** `index.html` en un navegador web
3. **¡Listo!** La aplicación está lista para usar

```bash
# Si tienes un servidor local, puedes usar:
python -m http.server 8000
# O con Node.js:
npx http-server
```

## 📖 Cómo Usar la Aplicación

### Crear una Nueva Tarea

1. Completa el formulario "Nueva Tarea" en la sección superior:
   - **Título** (obligatorio): Breve descripción de la tarea
   - **Descripción** (opcional): Detalles adicionales
   - **Categoría** (obligatoria): Selecciona una categoría existente
   - **Prioridad** (obligatoria): Alta, Media o Baja
   - **Fecha de Vencimiento** (opcional): Cuándo debe completarse

2. Haz clic en "Añadir Tarea" para crear la tarea
3. La tarea aparecerá inmediatamente en la lista

### Gestionar Tareas

**Marcar como Completada**
- Haz clic en la casilla de verificación al lado de la tarea
- La tarea se mostrará con opacidad reducida y tachada

**Eliminar una Tarea**
- Haz clic en el botón "🗑️ Eliminar" en la tarea
- Confirma la eliminación en el modal

**Reordenar Tareas**
- Arrastra cualquier tarea a una nueva posición
- El orden se guarda automáticamente

### Buscar y Filtrar

**Buscador Rápido**
- Usa la barra de búsqueda para encontrar tareas por título o descripción
- Los resultados se actualizan mientras escribes

**Filtros de Estado**
- **Todas**: Muestra todas las tareas
- **Pendientes**: Solo tareas no completadas
- **Completadas**: Solo tareas terminadas

**Filtro por Prioridad**
- Selecciona Alta, Media o Baja para ver solo esas tareas
- Combina con otros filtros

**Filtro por Categoría**
- Haz clic en cualquier categoría en el sidebar derecho
- Vuelve a hacer clic para deseleccionar

### Ordenamiento

- Usa el selector "Ordenar por..." para cambiar el orden:
  - **Fecha de Vencimiento**: Tareas próximas a vencer primero
  - **Prioridad**: Tareas de alta prioridad primero
  - **Recientes**: Tareas creadas recientemente primero

### Gestionar Categorías

**Crear Nueva Categoría**
- Haz clic en "+ Nueva Categoría" en el sidebar
- Ingresa el nombre en el modal
- La categoría está disponible inmediatamente

**Ver Contadores**
- El número de tareas por categoría aparece en el badge junto al nombre

### Operaciones en Lote

**Eliminar Tareas Completadas**
- Haz clic en "Eliminar Completadas"
- Confirma la acción en el modal
- Se eliminarán todas las tareas marcadas como completadas

### Tema y Apariencia

**Cambiar Tema**
- Haz clic en el toggle de tema en la esquina superior derecha
- ☀️ = Modo claro
- 🌙 = Modo oscuro
- La preferencia se guarda automáticamente

## 💾 Persistencia de Datos

Todos los datos se guardan automáticamente en **LocalStorage** del navegador:
- Tareas y sus detalles
- Categorías personalizadas
- Preferencia de tema (claro/oscuro)

**Importante**: Los datos se guardan localmente en tu navegador y no se sincronizan con otros dispositivos o navegadores.

## 🎨 Diseño Visual

### Paleta de Colores

**Tema Claro**
- Fondo primario: Blanco (#ffffff)
- Fondo secundario: Gris claro (#f5f5f5)
- Texto principal: Oscuro (#1a1a1a)
- Acento: Púrpura indigo (#6366f1)

**Tema Oscuro**
- Fondo primario: Oscuro (#1a1a1a)
- Fondo secundario: Gris oscuro (#2d2d2d)
- Texto principal: Blanco (#ffffff)
- Acento: Púrpura indigo (#6366f1)

### Indicadores Visuales

- 🔴 **Prioridad Alta**: Rojo (#ef4444)
- 🟠 **Prioridad Media**: Naranja (#f97316)
- 🔵 **Prioridad Baja**: Azul (#3b82f6)
- ⚠️ **Tareas Vencidas**: Borde rojo y fondo de alerta

## 📱 Responsive Design

La aplicación es completamente responsive y se adapta a:
- 📱 **Dispositivos móviles** (480px y menos)
- 📲 **Tablets** (768px - 1024px)
- 💻 **Desktops** (1200px y más)

### Cambios Responsive

- En móviles, el sidebar se reorganiza
- Los filtros se apilan verticalmente en pantallas pequeñas
- Los botones se hacen más grandes en móvil
- El grid principal se adapta automáticamente

## 🔒 Seguridad

- **Escapado de HTML**: Todas las entradas de usuario se escapan para prevenir inyecciones XSS
- **Validación de formularios**: Se validan los campos requeridos
- **Sin conexión externa**: No se envían datos a servidores externos
- **LocalStorage local**: Los datos permanecen en tu navegador

## 📊 Estructura del Código

### Clase Principal: `TodoApp`

La aplicación usa una clase `TodoApp` que maneja:

```javascript
class TodoApp {
  // Propiedades
  - tasks: Array de tareas
  - categories: Array de categorías
  - currentFilter: Filtro activo
  - darkMode: Estado del tema
  
  // Métodos principales
  - init(): Inicializa la aplicación
  - addTask(): Crea una nueva tarea
  - deleteTask(): Elimina una tarea
  - toggleTaskComplete(): Marca/desmarca una tarea
  - getFilteredTasks(): Filtra tareas según criterios
  - render(): Renderiza toda la interfaz
  - saveToLocalStorage(): Guarda datos
  - loadFromLocalStorage(): Carga datos
}
```

## 🐛 Resolución de Problemas

### Los datos desaparecen al cerrar la pestaña
- **Solución**: Los datos se guardan en LocalStorage. Si la pestaña se cierra correctamente, se guardan. Si se fuerza el cierre, podrían perderse cambios recientes.

### Las tareas no aparecen después de crear
- **Solución**: Asegúrate de llenar todos los campos requeridos (título y categoría)

### El modo oscuro no se mantiene
- **Solución**: Las cookies de terceros o la limpieza de caché pueden afectar LocalStorage. Intenta nuevamente.

### Las fechas se muestran en otro idioma
- **Solución**: Esto es normal. Las fechas se muestran en formato local de España (es-ES)

## 🚀 Mejoras Futuras Posibles

- ☁️ Sincronización en la nube
- 🔄 Importar/Exportar datos (JSON, CSV)
- 📧 Notificaciones de tareas vencidas
- 👥 Colaboración en tareas compartidas
- 📱 Aplicación móvil nativa
- 🎯 Subtareas y checklists
- 📈 Análisis y reportes de productividad
- 🔔 Recordatorios por email o notificación del navegador

## 📄 Licencia

Este proyecto es de código abierto y está disponible para uso personal y educativo.

## 👨‍💻 Autor

Desarrollado como una aplicación web moderna con HTML, CSS y JavaScript vanilla.

---

**¡Disfruta organizando tus tareas! 🎉**

Para reportar problemas o sugerir mejoras, considera mantener el código actualizado.
