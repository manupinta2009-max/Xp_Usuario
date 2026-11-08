# 📖 Proyecto: Mi Recetario (Experiencia de Usuario)

### 🎓 TRABAJO FINAL: EXPERIENCIA DE USUARIO
* **Clase:** 2.º Bachillerato · Segundo Parcial · Noviembre 2026
* **Centro educativo:** UTU María Espínola Espínola
* **Grupo:** BT Tecnología de la Información
* **Estudiantes:**
  * Rodrigo Alonso
  * Tiago Mussini
  * Manuel Pintaluba
* **Docente:** Bruno de San Vicente
* **Fecha de entrega:** Lunes 9 de Noviembre
* **Repositorio GitHub:** [https://github.com/manupinta2009-max/Xp_Usuario](https://github.com/manupinta2009-max/Xp_Usuario)

---

### 💡 Sobre este proyecto
Este trabajo fue desarrollado para la materia de **Experiencia de Usuario (UX)**. 

Queremos aclarar desde el inicio que el proyecto **no fue pensado como una página web terminada para el público en general ni como un producto comercial**. Se trata de un prototipo interactivo orientado a poner en práctica conceptos de usabilidad, diseño de interfaces y accesibilidad.

El objetivo fue tomar una situación real y cotidiana —estar en la cocina preparando una comida con un dispositivo al lado— e investigar cómo el diseño y los detalles de interacción pueden facilitarle las cosas a quien está cocinando: poder tachar ingredientes usados, buscar preparaciones con lo que hay en la heladera, evitar que se pierdan datos por toques accidentales y ofrecer una lectura clara y descansada.

---

## 📌 1. Ficha del Proyecto
* **Nombre:** Mi Recetario — Libreta Digital de Cocina.
* **Propósito:** Prototipo enfocado en experimentar con soluciones de Experiencia de Usuario (UX) e interfaz (UI) para la consulta y organización de recetas.
* **Modalidad de funcionamiento:** Aplicación ejecutada íntegramente en el navegador (*Client-side*), utilizando HTML, CSS y JavaScript nativo.
* **Manejo de datos:** Al ser un ejercicio práctico sin servidores ni backend externo, la persistencia se realiza localmente en el navegador a través de `localStorage`, sumando herramientas para exportar e importar la información en archivos `.json`.

---

## 🚀 2. Qué se puede hacer en el prototipo

### 📋 Gestión de Recetas
* **Cargar recetas:** Ventana modal sencilla para ingresar título, categoría, ingredientes, preparación, foto y datos clave.
* **Editar sin complicaciones:** Botón para abrir la receta en el formulario, ajustar cualquier detalle y guardar los cambios.
* **Confirmación para borrar:** Si tocás el botón de eliminar, se pide confirmación antes de borrar para no perder nada por error.
* **Datos rápidos de cocina:** Etiquetas visibles de tiempo estimado de preparación, porciones y dificultad (*Fácil, Media, Difícil*).

### 🍳 Asistente para el momento de cocinar
* **Checklist de ingredientes:** Podés ir marcando con un toque cada ingrediente a medida que lo vas agregando a la olla; queda tachado suavemente para no perderte.
* **Tarjetas plegables:** La preparación se despliega con el botón *"Ver preparación e ingredientes"*, manteniendo la pantalla limpia y ordenada.
* **Ficha para imprimir:** Genera una versión limpia de la receta, pensada para imprimir en papel o guardar en PDF sin que salgan los botones ni la barra de navegación.

### 🔍 Búsqueda y Organización
* **Búsqueda por nombre y por ingredientes:** Si ponés *"papas"* o *"huevo"*, busca tanto en el título como dentro de la lista de ingredientes de cada receta.
* **Filtros por categoría:** Filtrado al instante por *Entrada, Plato principal, Postre, Bebida u Otro*.
* **Favoritos (⭐):** Marcá las recetas que más uses con la estrella y filtralas cuando quieras con el botón *"Favoritos"*.

### 💾 Manejo de Fotos y Respaldo
* **Ajuste automático de imágenes:** Al subir una foto, la aplicación la redimensiona y comprime en el momento para no saturar la memoria local del navegador ni poner lenta la interfaz.
* **Exportar recetas (JSON):** Descarga un archivo con las recetas guardadas para tener una copia de seguridad.
* **Importar recetas:** Permite cargar ese archivo en cualquier otro navegador para recuperar o mover las recetas.

### 🌓 Interfaz y Adaptabilidad
* **Modo Claro y Oscuro:** Selector en la barra superior (☀️ / 🌙) para que la pantalla no moleste a la vista en ambientes con poca luz.
* **Diseño adaptable:** Funciona cómodamente tanto en computadoras como en tablets y celulares.
* **Mensaje cuando no hay resultados:** Si la búsqueda no coincide con ninguna receta, muestra un aviso claro y amigable en vez de dejar la pantalla vacía.

---

## 🎨 3. Criterios de Experiencia de Usuario (UX/UI) que aplicamos

* **Evitar errores accidentales:** El diálogo antes de borrar una receta previene que se pierda información por un toque involuntario en la pantalla.
* **Cargar fotos sin trabas:** El usuario no tiene que preocuparse por el tamaño o peso de la foto; la interfaz la procesa directo en el navegador.
* **Respuesta visual clara:** Los botones y casillas responden de inmediato al tacto o al pasar el cursor, dando la seguridad de que la acción se registró.
* **Tipografías legibles y adecuadas:** Usamos *Playfair Display* para títulos gastronómicos cálidos y *Plus Jakarta Sans* para que los ingredientes y las instrucciones se lean con total claridad, incluso a cierta distancia.
* **Pensado para usar en la cocina:** Botones con buen tamaño para tocar fácilmente desde el celular y modo oscuro para cuidar la vista en horarios nocturnos.

---

## 🛠️ 4. Tecnologías Utilizadas

* **HTML5:** Estructuración semántica con elementos nativos (`<header>`, `<main>`, `<dialog>`, `<details>`, `<summary>`).
* **CSS3:**
  * Variables CSS para cambiar fácilmente entre tema claro y oscuro.
  * Flexbox y CSS Grid para que el diseño se adapte a cualquier pantalla.
  * Estilos de impresión específicos con `@media print`.
* **JavaScript Nativo (ES6+):**
  * Manejo del DOM y eventos en tiempo real sin librerías externas.
  * API `localStorage` para guardar las recetas y el tema seleccionado en el navegador.
  * API `Canvas` para redimensionar y optimizar las fotografías.
  * `FileReader` y `Blob` para la exportación e importación del archivo JSON.
* **Google Fonts:** Tipografías *Playfair Display* y *Plus Jakarta Sans*.

---

## 🎤 5. Guía para la Demostración en Clase

Para la presentación del trabajo ante el docente y el grupo, este es el recorrido que pensamos:

1. **Introducción breve:**
   * Contar el objetivo del trabajo: explorar la experiencia de usuario (UX) en una libreta de recetas pensada para usar mientras se cocina.
   * Mostrar el diseño general, la organización visual y el estilo de las tarjetas.

2. **Búsqueda y filtros:**
   * Escribir un ingrediente (como *"papas"*) para mostrar cómo el buscador encuentra recetas por lo que tenemos a mano y no solo por el título.
   * Probar el filtro de categorías y marcar una receta como favorita (⭐).

3. **Uso en plena cocina:**
   * Desplegar una receta y marcar ingredientes en el checklist para simular el paso a paso de una preparación.
   * Tocar el botón *"Imprimir"* para ver cómo se genera la ficha limpia sin botones de la interfaz.

4. **Carga y edición:**
   * Mostrar el formulario para añadir una receta con sus datos (tiempo, porciones, dificultad).
   * Cargar una foto para mostrar cómo se procesa automáticamente.
   * Editar una receta y luego mostrar el aviso de confirmación que aparece si intentamos borrarla.

5. **Modo oscuro y respaldo:**
   * Cambiar entre modo claro y oscuro con el botón de la cabecera.
   * Mostrar la opción de exportar las recetas a un archivo `.json` de respaldo.

---

## 📁 6. Estructura de Archivos

* `Codigo/index.html`: Archivo principal con la estructura, estilos y lógica del recetario.
* `Codigo/recetas.html`: Copia sincronizada del archivo de la aplicación.
* `Codigo/tortilla.jpg`: Foto de muestra utilizada para la receta inicial de Tortilla de papas.
* `Docs/Como_Funciona.md`: Explicación sencilla del funcionamiento y las decisiones tomadas en el diseño.
* `Docs/Stack.md`: Resumen técnico de las tecnologías, herramientas y recursos utilizados.
* `README.md`: Presentación general del proyecto y guía para la clase.
