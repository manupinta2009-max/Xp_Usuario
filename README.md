# 📖 Proyecto: Mi Recetario (Experiencia de Usuario)

### 🎓 TRABAJO FINAL: EXPERIENCIA DE USUARIO
* **Clase:** 2.º Bachillerato · Segundo Parcial · Noviembre 2026
* **Centro educativo:** UTU María Espínola Espínola
* **Grupo:** BT Tecnología de la Información
* **Estudiantes:**
  * Rodrigo Alonso
  * Tiago Mussini
  * Manuel Pintaluba
* **Docente:** Burno de San Vicente
* **Fecha de entrega:** Lunes 9 de Noviembre
* **Repositorio GitHub:** [https://github.com/manupinta2009-max/Xp_Usuario](https://github.com/manupinta2009-max/Xp_Usuario)

---

### 🌟 Bienvenida al Proyecto
¡Bienvenidos a nuestra web! Este es un espacio creado para compartir nuestra pasión por la cocina. Acá cada persona puede publicar sus propias recetas, compartir sus preparaciones y descubrir nuevas ideas de otras personas.

La idea es que todos puedan aportar algo, desde recetas sencillas para el día a día hasta preparaciones más elaboradas. Queremos crear una comunidad donde podamos aprender, inspirarnos y disfrutar de la cocina juntos.

¡Compartí tus recetas, descubrí nuevas ideas y dejá que otros conozcan tus creaciones!

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
  * CSS Grid y Flexbox responsivo.
  * Animaciones suaves con curvas de aceleración cubic-bezier.
  * Reglas para medios impresos (`@media print`).
* **JavaScript Moderno (ES6+):**
  * Manipulación reactiva del DOM sin librerías externas.
  * API `localStorage` para almacenamiento persistente.
  * API `HTMLCanvasElement` para compresión y optimización de imágenes en el cliente.
  * API `FileReader` y `Blob` para exportar e importar datos en formato JSON.
* **Tipografías de Google Fonts:**
  * *Playfair Display* (títulos con personalidad gastronómica).
  * *Plus Jakarta Sans* (textos técnicos y legibilidad).

---

## 🎤 5. Guía de Presentación Paso a Paso (Demostración en Vivo para la Clase)

Para presentar el proyecto ante el docente y compañeros de clase, sugerimos seguir este orden demostrativo:

1. **Apertura e Introducción:**
   * Explicar el objetivo del proyecto: crear un recetario enfocado en la experiencia de usuario real mientras se cocina.
   * Mostrar el diseño visual general, la paleta cálida y la jerarquía de las tarjetas.

2. **Demostración de Búsqueda y Filtros:**
   * Escribir *"papas"* en el buscador para demostrar que busca dentro de los ingredientes y no solo en el título.
   * Filtrar por categoría (*Plato principal*).
   * Marcar la receta con la estrella (⭐) y presionar el botón *"Favoritos"*.

3. **Demostración del Asistente en la Cocina:**
   * Abrir el acordeón *"Ver preparación e ingredientes"*.
   * Tocar los checkboxes para simular cómo se tachan los ingredientes ya usados mientras se cocina.
   * Presionar el botón *"Imprimir"* para mostrar cómo se genera una ficha limpia para papel o PDF sin barras ni botones.

4. **Demostración de Creación y Edición:**
   * Abrir el modal *"Añadir receta"* y mostrar los metadatos (tiempo, porciones, dificultad).
   * Cargar una foto pesada y explicar cómo la web la comprime automáticamente sin trabarse.
   * Editar una receta existente para comprobar que no se pierden datos.
   * Intentar eliminar una receta para mostrar el diálogo de confirmación que previene errores del usuario.

5. **Demostración de Modo Oscuro y Respaldo:**
   * Tocar el botón 🌙 en la cabecera para alternar a tema oscuro y explicar la ventaja al cocinar con poca luz.
   * Presionar *"Exportar"* para descargar el archivo `.json` de respaldo.

---

## 📁 6. Estructura de Archivos

* `Codigo/index.html`: Archivo principal con la aplicación web completa (HTML, CSS y JavaScript integrados).
* `Codigo/recetas.html`: Copia sincronizada del código de la aplicación.
* `Codigo/tortilla.jpg`: Fotografía optimizada para la receta inicial de Tortilla de papas.
* `Docs/Como_Funciona.md`: Guía explicativa para personas sin conocimientos de código.
* `Docs/Stack.md`: Ficha técnica del Stack Tecnológico del proyecto.
* `README.md`: Este documento de presentación y guía técnica para la clase.
