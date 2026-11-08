# 🍳 ¿Cómo Funciona Mi Recetario?
### *Guía de funcionamiento y decisiones de diseño del proyecto*

---

## 🌟 ¿De qué trata este proyecto?

**Mi Recetario** es un prototipo desarrollado para la materia de **Experiencia de Usuario (UX)**. La idea detrás de este trabajo no fue crear una plataforma web definitiva para el público en general ni competir con servicios online, sino poner el foco en la interacción: pensar cómo una persona usa una libreta de recetas en una situación real (en plena cocina) y ver qué detalles de diseño hacen que esa tarea sea más fácil y cómoda.

Todo el funcionamiento se pensó desde el punto de vista de quien cocina: que la pantalla no se llene de cosas innecesarias, que sea rápida de consultar y que no te complique con registros ni pasos de más.

---

## 📸 1. Manejo de fotos sin complicaciones

Cuando querés sumar una foto a una receta, muchas veces las imágenes que sacamos con el celular pesan varios megabytes. 

* Para que la página no se vuelva lenta ni consuma demasiada memoria del navegador, implementamos un proceso que reduce y ajusta la foto directamente en el dispositivo en el momento en que la seleccionás.
* De esa forma la imagen se ve bien en las tarjetas, pero ocupa una fracción mínima del espacio y carga al instante.

---

## 🔍 2. Búsqueda por nombre o por lo que tengas a mano

A veces uno sabe exactamente qué receta quiere buscar, pero otras veces abrís la heladera, ves un par de ingredientes y querés saber qué podés preparar.

* La barra de búsqueda revisa tanto el **título de la receta** como la **lista de ingredientes**.
* Si escribís *"papas"* o *"cebolla"*, la pantalla te muestra enseguida qué preparaciones las incluyen.
* Además, podés filtrar rápido por categorías (*Entrada, Plato principal, Postre, Bebida u Otro*) o ver solo las que marcaste como favoritas con la estrella (⭐).

---

## 👨‍🍳 3. Asistente práctico para el momento de cocinar

Estar cocinando con las manos ocupadas o con comida en la mesada cambia la forma en que interactuás con la pantalla. Por eso sumamos detalles pensados para ese momento:

* **Tarjetas plegables:** Cada receta muestra solo lo esencial para no saturar la vista. Con el botón *"Ver preparación e ingredientes"* desplegás los pasos solo cuando los necesitás.
* **Casillas para tachar ingredientes:** Cada ingrediente tiene una casilla para marcarlo a medida que lo vas usando. Al tocarlo queda tachado en gris claro, lo que ayuda a no dudar si ya agregaste la sal, el aceite o cualquier otro ingrediente.
* **Datos rápidos de referencia:** En la cabecera de la receta se ven directo el tiempo estimado, las porciones que rinde y la dificultad.

---

## 🌙 4. Modo Claro y Modo Oscuro

* En la esquina superior derecha hay un botón para alternar entre el tema claro (☀️) y el tema oscuro (🌙).
* Esto ayuda a no cansar la vista si estás cocinando de noche o con poca iluminación, y el navegador recuerda tu elección para la próxima vez que abras el proyecto.

---

## 🖨️ 5. Ficha limpia para imprimir

Aunque estemos usando una pantalla, a veces es más cómodo tener la receta en una hoja sobre la mesada para no ensuciar el teléfono o la computadora:

* Cada receta tiene un botón **"Imprimir"**.
* En lugar de mandar a imprimir toda la página con botones y menús, preparamos un diseño específico de impresión que saca una ficha limpia y ordenada, lista para imprimir o guardar como PDF.

---

## 💾 6. Respaldo de datos (Exportar e Importar)

Al tratarse de un prototipo que guarda la información en la memoria local del navegador (`localStorage`), las recetas se conservan en ese dispositivo pero no se sincronizan automáticamente con otros.

* Para solucionar esto de forma práctica, sumamos dos botones:
  * **Exportar:** Descarga un archivo sencillo (`.json`) con todas las recetas que tengas cargadas.
  * **Importar:** Te permite seleccionar ese archivo en otro navegador o computadora para recuperar tus recetas rápidamente.

---

## 🛡️ 7. Prevención de errores comunes

* Para evitar pérdidas accidentales, si tocás *"Eliminar"* en una receta la aplicación te pide confirmación antes de borrarla.
* Si te equivocaste en un paso o querés cambiar una cantidad, podés tocar *"Editar"* en cualquier momento para modificar los datos directamente en el formulario sin tener que cargar la receta de vuelta.
