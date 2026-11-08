# Stack Tecnológico y Herramientas

Resumen de las tecnologías, herramientas y recursos utilizados en el desarrollo de este prototipo para la materia de Experiencia de Usuario.

#### IAs de apoyo durante el desarrollo
| Herramienta | Rol en el proyecto |
| :--- | :--- |
| Gemini | Consultas de diseño, búsqueda de información y análisis |
| ChatGPT | Apoyo en la redacción de documentación y consultas conceptuales |
| Claude | Sugerencias sobre flujo de experiencia de usuario (UX) |
| Antigravity | Asistencia en código, refactorización visual y ajustes de interfaz |

#### Lenguajes
| Lenguaje | Uso en el proyecto |
| :--- | :--- |
| HTML5 | Estructura semántica de la página (`<header>`, `<main>`, `<dialog>`, `<details>`, `<summary>`) |
| CSS3 | Diseño visual, variables para modo claro/oscuro, diseño adaptable y estilos de impresión |
| JavaScript (ES6+) | Lógica de la interfaz: interacción con el usuario, filtros, modal y guardado de datos |

#### APIs nativas del navegador
| API Web | Uso en el proyecto |
| :--- | :--- |
| `localStorage` | Guardado local de las recetas y de la preferencia de tema (claro / oscuro) |
| Canvas API | Ajuste y compresión del tamaño de las fotos al momento de subirlas |
| FileReader y Blob | Lectura del archivo de recetas y descarga de copias de seguridad en formato JSON |
| HTML5 Dialog API | Ventanas emergentes nativas para el formulario y la confirmación antes de borrar |
| Print API (`window.print`) | Apertura del diálogo de impresión con el formato limpio de la receta |

#### Diseño e Interfaz (UI/UX)
| Recurso | Uso en el proyecto |
| :--- | :--- |
| CSS Grid y Flexbox | Organización flexible de los elementos para que se vean bien en celular y PC |
| Variables CSS | Paletas de colores centralizadas para cambiar fácilmente entre tema claro y oscuro |
| Google Fonts (Playfair Display) | Tipografía para los títulos |
| Google Fonts (Plus Jakarta Sans) | Tipografía limpia y clara para facilitar la lectura de ingredientes y pasos |
| SVG | Iconos vectoriales livianos integrados directamente en el código |

#### Manejo de Datos y Enfoque Técnico
| Aspecto | Detalle |
| :--- | :--- |
| Formato JSON | Formato en el que se estructuran las recetas y se exportan/importan los respaldos |
| Enfoque del prototipo | Ejecución directa en el navegador (*Client-side*), guardando en la memoria local para probar la experiencia de uso sin necesidad de montar una infraestructura de backend |
