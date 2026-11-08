# 🍳 ¿Cómo Funciona Mi Recetario?
### *Guía sencilla explicada para todo público (sin tecnicismos de programación)*

---

## 🌟 ¿Qué es esta aplicación?

**Mi Recetario** es una libreta de cocina digital interactiva. Su objetivo principal es ayudarte a organizar, consultar y seguir el paso a paso de tus platos favoritos de forma cómoda, limpia y sin complicaciones mientras estás cocinando.

Está diseñada pensando 100% en la **Experiencia de Usuario (UX)**: es intuitiva, rápida y no te obliga a registrarte, recordar contraseñas ni lidiar con publicidad molesta.

---

## 🔒 1. ¿Dónde se guardan mis recetas? (Sin servidores ni cuentas)

A diferencia de las páginas web tradicionales que envían tus datos a computadoras en otros países:

* **Tus recetas viven en tu propio dispositivo:** Ya sea que uses tu computadora, tablet o teléfono, la aplicación utiliza una memoria interna segura de tu navegador llamada *Almacenamiento Local* (`localStorage`).
* **Privacidad total:** Nadie más en internet puede ver lo que escribes; es como tu recetario físico personal en tu mesada.
* **Funciona sin conexión (Offline):** Una vez que abres la página, puedes desconectarte de internet o poner el teléfono en modo avión y la aplicación seguirá funcionando con normalidad.

---

## 📸 2. La magia con las fotografías: compresión automática

En muchas páginas, si subes una foto pesada sacada con una cámara moderna, la web se vuelve lenta o se traba.

* **¿Qué hace nuestra página entre bastidores?** En cuanto seleccionas una foto de tu plato, la página la procesa en milisegundos directamente en la memoria de tu dispositivo:
  1. La redimensiona a un tamaño equilibrado para pantalla.
  2. Reduce su peso sin perder calidad visible.
  3. La guarda optimizada para que tu libreta nunca se sature de espacio.

---

## 🔍 3. Búsqueda inteligente: encuentra por lo que tienes en la heladera

¿Tienes papas y huevos y no sabes qué cocinar?

* La barra de búsqueda busca en dos lugares al mismo tiempo: en el **título de la receta** y en la **lista de ingredientes**.
* Con solo escribir una palabra (por ejemplo: *"aceite"* o *"cebolla"*), la pantalla filtra en vivo y te muestra solo las preparaciones que llevan ese ingrediente.
* Además, puedes filtrar por momentos del menú: *Entradas, Platos principales, Postres o Bebidas*.

---

## 👨‍🍳 4. El Asistente de Cocina: una ayuda práctica mientras cocinas

Diseñamos la interfaz para evitar accidentes y manchas en la pantalla:

* **Tarjetas plegables:** Cada receta se mantiene ordenada en una tarjeta compacta. Toca *"Ver preparación e ingredientes"* para desplegarla cuando estés listo.
* **Lista de compras y preparación interactiva (Checklist):** Cada ingrediente tiene una casilla de verificación. A medida que vas pesando o agregando un ingrediente a la olla, lo tocas y queda tachado en gris suave. Así nunca te preguntarás si ya le pusiste sal o levadura.
* **Metadatos rápidos:** En un solo vistazo ves el **tiempo** aproximado de cocción, las **porciones** que rinde y la **dificultad** técnica del plato.

---

## 🌙 5. Modo Claro y Modo Oscuro: cuidando tu vista

* En la esquina superior derecha encontrarás un botón con un sol ☀️ o una luna 🌙.
* Si estás cocinando de noche o en una cocina con luz tenue, activa el **Modo Oscuro** para relajar la vista y ahorrar batería en pantallas de celular. La página recordará tu preferencia para la próxima vez que entres.

---

## 🖨️ 6. Ficha de impresión limpia (para la abuela o para pegar en la heladera)

Si prefieres tener la receta en papel o guardarla como PDF:

* Cada tarjeta incluye un botón **"Imprimir"**.
* En lugar de imprimir toda la página web con botones y menús, genera automáticamente una ficha tipográfica limpia, elegante y formateada especialmente para hojas A4.

---

## 💾 7. Copias de seguridad: lleva tus recetas a cualquier lado

¿Quieres pasarle tus recetas a un familiar o cambiar de celular?

* **Exportar (Descargar):** Toca *"Exportar"* y se descargará un archivito `.json` con todas tus recetas guardadas.
* **Importar (Restaurar):** En el otro dispositivo, abre la página, toca *"Importar"*, selecciona ese archivito y listo: todas tus recetas se cargarán al instante.

---

## 🛡️ 8. Prevención de errores accidentales

* Si tocas *"Eliminar"* por descuido, la página no borra la receta de inmediato: abre una ventana de diálogo para que confirmes si realmente deseas quitarla, evitando que pierdas tus anotaciones por un clic en falso.
* Puedes editar cualquier dato o ingrediente en cualquier momento tocando *"Editar"*, sin necesidad de empezar de cero.
