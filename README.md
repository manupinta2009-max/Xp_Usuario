# 📖 Proyecto: Mi Recetario (Experiencia de Usuario)

### 👨‍🎓 Datos de Presentación
* **Institución:** UTU (Universidad del Trabajo del Uruguay)
* **Asignatura:** Experiencia de Usuario (UX / UI)
* **Proyecto:** Mi Recetario — Colección Gastronómica Personal
* **Estudiante:** Manuel Pintado (`manupinta2009-max`)
* **Repositorio GitHub:** [https://github.com/manupinta2009-max/Xp_Usuario](https://github.com/manupinta2009-max/Xp_Usuario)
* **Fecha:** Noviembre 2026

Documento de presentación y guía técnica del proyecto **Mi Recetario**, desarrollado para la asignatura de **Experiencia de Usuario (UX/UI)** en **UTU**.

---

## 📌 1. Ficha del Proyecto
* **Nombre del proyecto:** Mi Recetario — Colección Gastronómica Personal.
* **Propósito:** Aplicación web interactiva pensada para el uso cotidiano en la cocina, priorizando la facilidad de uso, la velocidad y una experiencia de usuario (UX) limpia y atractiva.
* **Arquitectura:** 100% del lado del cliente (*Client-side*), sin frameworks pesados ni dependencias externas; funciona de manera autónoma y *offline-first*.
* **Almacenamiento:** Persistencia de datos en el propio navegador mediante la API de `localStorage`.

---

## 🚀 2. Lista Completa de Funcionalidades

### 📋 Gestión de Recetas
* **Crear recetas:** Formulario modal intuitivo para ingresar título, categoría, ingredientes, preparación y foto.
* **Editar recetas existentes:** Botón *"Editar"* que precarga los datos en el modal para modificarlos en cualquier momento sin perder información.
* **Eliminación protegida:** Diálogo de confirmación antes de eliminar para prevenir pérdidas accidentales de recetas.
* **Metadatos culinarios:** Etiquetas de **tiempo de preparación** (ej: *35 min*), **porciones** (ej: *4 porc.*) y **dificultad** (*Fácil, Media, Difícil*).

### 🍳 Asistente Interactivo de Cocina
* **Checklist interactivo de ingredientes:** Casillas de verificación para marcar y tachar los ingredientes ya utilizados mientras se cocina.
* **Acordeón desplegable:** Contenido estructurado que mantiene las tarjetas compactas y legibles en la pantalla principal.
* **Ficha de impresión individual:** Genera una hoja limpia lista para imprimir en papel o guardar en PDF (sin menús ni botones molestos).

### 🔍 Organización y Filtros
* **Búsqueda en tiempo real bi-direccional:** Filtra instantáneamente tanto por el **nombre de la receta** como por **cualquier ingrediente** que contenga (ej. *"papas"* o *"huevo"*).
* **Filtrado por categorías:** Clasificación inmediata por *Entrada, Plato principal, Postre, Bebida u Otro*.
* **Sistema de favoritos (⭐):** Permite marcar recetas destacadas con un clic y filtrarlas con el botón *"Favoritos"*.

### 💾 Almacenamiento y Portabilidad
* **Compresión automática de imágenes:** Redimensiona y optimiza las fotos subidas mediante la API de Canvas antes de guardarlas, evitando saturar el límite de almacenamiento de `localStorage`.
* **Exportar copia de seguridad (JSON):** Descarga toda la base de datos de recetas en un archivo estándar `.json`.
* **Importar copia de seguridad:** Permite cargar y restaurar recetas desde cualquier archivo JSON previamente exportado.

### 🌓 Interfaz y Accesibilidad
* **Modo Claro / Modo Oscuro (Dark Mode):** Interruptor en la cabecera (☀️ / 🌙) con guardado automático de la preferencia del usuario.
* **Diseño adaptativo (Responsive Design):** Interfaz optimizada para celulares, tablets y computadoras de escritorio.
* **Estado vacío amigable:** Ilustración y mensaje explicativo cuando una búsqueda no arroja resultados.

---

## 🎨 3. Principios de Experiencia de Usuario (UX/UI) Aplicados

* **Prevención de errores del usuario:** El modal de confirmación antes de borrar evita acciones destructivas involuntarias.
* **Reducción de fricción:** El usuario no necesita redimensionar sus fotos con programas externos; la app las comprime automáticamente en el navegador.
* **Retroalimentación inmediata (Feedback visual):** Microinteracciones en botones (*hover*, *active*), cambio instantáneo del estado de los checkboxes y animaciones suaves.
* **Jerarquía tipográfica:** Combinación equilibrada entre *Playfair Display* (elegancia editorial) y *Plus Jakarta Sans* (alta legibilidad técnica).
* **Accesibilidad visual:** Contrastes de color certificados y soporte para modo oscuro pensado para ambientes con poca luz en la cocina.
* **Diseño táctil:** Botones con áreas de toque amplias (mínimo 44px) ideales para su uso en teléfonos móviles mientras se manipulan alimentos.

---

## 🛠️ 4. Lista de Tecnologías Utilizadas

* **HTML5:** Marcado semántico (`<header>`, `<dialog>`, `<details>`, `<summary>`, `<main>`, `<input type="file">`).
* **CSS3 Moderno:**
  * Variables CSS nativas (*Design Tokens* para paleta clara y oscura).
  * Flexbox y CSS Grid para diagramación fluida.
  * Estilos de vidrio esmerilado (*Glassmorphism* con `backdrop-filter`).
  * Estilos `@media print` para formato de impresión en papel.
  * Animaciones mediante `@keyframes` y curvas de aceleración `cubic-bezier`.
* **JavaScript Vanilla (ES6+):**
  * Sin librerías ni frameworks (código nativo puro y liviano).
  * Delegación de eventos (*Event Delegation*) para optimizar el rendimiento del DOM.
  * Funciones de orden superior (`filter`, `map`, `reduce`, `find`).
* **APIs Nativas del Navegador:**
  * `localStorage API` (persistencia local sin base de datos).
  * `HTML Canvas API` (procesamiento y compresión gráfica).
  * `FileReader API` (lectura local de imágenes y archivos JSON).
  * `HTML Dialog API` (gestión accesible de ventanas modales).

---

## 🎤 5. Guion Sugerido para la Demostración en Clase (Paso a Paso)

1. **Introducción (1 min):** Mostrar la interfaz inicial, la tarjeta por defecto (*Tortilla de papas*) y explicar el concepto de recetario personal rápido.
2. **Interactividad en cocina (1 min):** Desplegar la receta y mostrar el checklist interactivo marcando ingredientes usados.
3. **Búsqueda inteligente (1 min):** Escribir *"papas"* en el buscador para demostrar que busca tanto por nombre como por ingredientes.
4. **Modo Oscuro (30 seg):** Tocar el botón de tema (☀️/🌙) y mostrar la adaptación de colores y contraste.
5. **Carga y compresión de imagen (1 min):** Crear una receta nueva, subir una fotografía y explicar que la imagen se optimiza automáticamente para no saturar la memoria local.
6. **Edición y borrado seguro (1 min):** Modificar la receta creada y luego demostrar el diálogo de confirmación de eliminación.
7. **Portabilidad de datos (30 seg):** Presionar *"Exportar"* para descargar el archivo JSON y mostrar cómo se respalda la información.

---

## 💻 6. ¿Cómo Ejecutar el Proyecto?

* **Opción directa:** Hacer doble clic sobre `Codigo/index.html` para abrirlo en cualquier navegador (Firefox, Chrome, Edge, Safari).
* **Opción con servidor local:**
  ```bash
  cd Codigo
  python3 -m http.server 8000
  ```
  Abrir en el navegador: `http://localhost:8000`

---

## 📁 7. Estructura de Archivos

* `Codigo/index.html`: Archivo principal con la aplicación completa (HTML + CSS + JavaScript integrados).
* `Codigo/recetas.html`: Copia sincronizada del código de la aplicación.
* `README.md`: Este documento de presentación para la clase.