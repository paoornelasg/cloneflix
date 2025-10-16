# 🎬 CloneFlix (mini clon de Netflix)

## 🧩 Introducción
**CloneFlix** es un mini clon de Netflix realizado con **HTML, CSS y JavaScript**. La app usa la API pública de TVMaze para mostrar series y películas en formato tipo carrusel, junto con un hero principal que incluye un botón de “Ver ahora”.  

Está construida con **Bootstrap 5** para la utilización de los estilos rápidos, y no involucra backend ni otras configuraciones, solo se necesita abrir el `index.html` en el navegador (o con un servidor local) y listo.

---

## ⚙️ Lenguajes, tecnologías y recursos utilizados
- **HTML5**, se usa para armar toda la estructura de la app (navbar, header, main, footer y modal).
- **CSS**, en el archivo `css/app.css` van los estilos globales, incluyendo fondo oscuro, colores, carruseles y detalles visuales del FrontEnd.  
- **JavaScript**, maneja toda la lógica, usando `fetch` para traer los datos desde la API de TVMaze y usar de forma dinámica las filas de contenido.  
- **Bootstrap 5**, ayuda a mantener un diseño responsivo, realizar los componentes y el modal de detalle.  
- **API** , [`https://api.tvmaze.com`](https://api.tvmaze.com) (es pública).  
  El *endpoint* base está definido en `app.js`, por lo que puede modificarse fácilmente para el uso de otros endpoints.

---

## 🗂️ Elementos y estructura del proyecto
El proyecto se encuentra estructurado como se muestra a continuación:

```
/
├─ index.html
├─ css
│  └─ app.css
└─ js
    └─ app.js
```
- `index.html`: esqueleto HTML; contiene el navbar de búsqueda, hero, contenedor de filas y modal de detalle. Realiza la carag de Bootstrap y enlaza los archivos de estilos y scripts para el uso de CSS y JS, respectivamente.
- `css/app.css`: se usa un color base oscuro, con un efecto de degradado en el hero, carruseles horizontales con scroll-snap, y tarjetas tipo póster.
- `js/app.js`: inicializa la app, hace `fetch` a TVMaze (`/shows?page=1`), y prepara `renderRow(...)` para construir secciones tipo “Tendencias”, mostrando las series y películas. Permite realizar búsquedas con `wireSearch(...)` y mostrar modales con los detalles de la serie/película de interés utilizando la función `openDetail(...)`.

---

## 👾 Aspectos relevantes del código
- Usa `fetch` para traer datos de TVMaze (`/shows?page=1`).
- Crea filas dinámicas con `renderRow()`.
- Utiliza `posterCard()` para crear las tarjetas en el rail.
- El hero se puede actualizar con un show aleatorio.
- Todo el scroll horizontal se maneja con `scroll-snap`.
- La búsqueda de series y películas se emplea a través de la función `wireSearch()` mapeando los datos obtenidos de la API y mostrando la fila dinámica. 
- Realiza el manejo de caracteres a través de las funciones `escapeHTML()` y `stripHTML()`.
- El modal permite mostrar detalles de las series y películas (tipo `Netflix`), mostrando la portada, título, género, descripción y status utiliando la función `openDetail()`.

---

## 📝 Otra documentación...
- ✓ Revisar cómo usarlo: [`Instalación`](./Instalacion.md)
- ✓ Código inicial: [`Versión 1`](./Codigo.md)
- ✓ Código actualizado: [`Versión 2`](./Codigo2.md)

---

## 📝 Créditos
- Proyecto hecho por Pao ❤️.
- Datos de series obtenidos de TVMaze (uso educativo). 
- Diseño con Bootstrap 5.