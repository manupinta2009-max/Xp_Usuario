# 📖 Mi Recetario

Una aplicación web moderna, ágil y visualmente atractiva para organizar, cocinar y conservar tus mejores preparaciones culinarias. No requiere instalación de servidores ni bases de datos externas; funciona 100% en el navegador utilizando almacenamiento local (`localStorage`).

---

## 🚀 Funcionalidades Principales

1. **Gestión de Recetas (Crear y Editar):**
   - Añade nuevas preparaciones o edita cualquier receta existente mediante una ventana modal interactiva.
   - Permite indicar título, categoría, ingredientes e instrucciones paso a paso.

2. **Metadatos Culinarios:**
   - Campos opcionales para **tiempo de preparación** (ej: *35 min*), **porciones** (ej: *4 porc.*) y **nivel de dificultad** (*Fácil, Media, Difícil*), visibles como etiquetas en cada tarjeta.

3. **Checklist Interactivo de Ingredientes:**
   - En el detalle de cada receta, los ingredientes se presentan con casillas de verificación para irlos marcando y tachando a medida que cocinas.

4. **Compresión Automática de Imágenes:**
   - Al seleccionar una foto para la receta, el sistema la optimiza y redimensiona automáticamente en el navegador mediante Canvas antes de guardarla, evitando llenar la memoria de `localStorage`.

5. **Búsqueda Inteligente y Filtros:**
   - **Búsqueda en tiempo real:** Encuentra recetas tanto por su nombre como por los ingredientes que contienen (ej. busca *"huevo"* o *"papas"*).
   - **Filtro por categoría:** Filtra por *Entrada, Plato principal, Postre, Bebida u Otro*.
   - **Filtro de Favoritos (⭐):** Marca tus recetas favoritas y visualízalas con un solo clic.

6. **Confirmación de Eliminación:**
   - Diálogo de seguridad para evitar borrar recetas de forma accidental.

7. **Modo Claro y Oscuro (Dark Mode):**
   - Interruptor de tema (☀️/🌙) en el encabezado con transición suave, adaptado para cocinar de noche y guardado en preferencias.

8. **Copia de Seguridad (Exportar / Importar JSON):**
   - Descarga todas tus recetas en un archivo `.json` para respaldarlas o compartirlas, y cárgalas en cualquier momento con un clic.

9. **Modo de Impresión (Ficha de Cocina):**
   - Botón individual de impresión por receta o mediante `Ctrl + P`, formateado limpiamente sin barras ni botones para imprimir en papel o guardar en PDF.

---

## 💻 ¿Cómo ejecutar el proyecto?

No requiere instalar dependencias:

- **Opción rápida:** Abre el archivo `Codigo/index.html` haciendo doble clic desde tu administrador de archivos.
- **Con servidor local (opcional):**
  ```bash
  cd Codigo
  python3 -m http.server 8000
  ```
  Luego ingresa a `http://localhost:8000` en tu navegador.

---

## 📁 Estructura del Repositorio

- `Codigo/index.html`: Aplicación web completa (HTML5, CSS3 moderno y JavaScript Vanilla).
- `Codigo/recetas.html`: Copia de respaldo del código de la aplicación.
- `README.md`: Documentación del proyecto.