# 🛠️ Instalación y requisitos  

Correr CloneFlix es sencillo y rápido sin necesidad de utilizar configuraciones o aplicaciones externas. Solo deben seguirse estos pasos:  

---

## ⚙️ Requisitos
- Un navegador moderno (Chrome, Edge, Firefox, Opera…).  
- Opcional: servidor local para que todo funcione sin errores de rutas.  
  Se puede utilizar:  
  - VS Code y Live Server.
  - Cualquier otra app que funcione como servidor local.

---

## 👾 Cómo correrlo  
1. Descargar o clonar el repositorio [https://github.com/paoornelasg/cloneflix.git](https://github.com/paoornelasg/cloneflix.git).  
2. Abrir la carpeta en el editor (VS Code, por ejemplo).  
3. Iniciar el servidor:  
   - Con Live Server: clic derecho en `index.html` y,posteriormente, click en *Open with Live Server*.  
4. Abrir el navegador en [http://localhost:5500](http://localhost:5500) (o el puerto que aparezca) y revisar:  
   - Que se cargue el hero.  
   - Que aparezcan los carruseles con scroll horizontal.  
   - Que el modal funcione adecuadamente.  

---

## 🌐 Sobre la API  
CloneFlix usa la API pública de TVMaze y hace peticiones básicas:  
- Listado general → `/shows?page=1`  
- Búsqueda → `/search/shows?q=TU_TEXTO`  

El enlace que es la base está definido en `js/app.js` en la constante `API`, así que para probear otra api solo se necesita cambiar esa parte.  

Y listo, ya se puede utilizar el mini clon de Netflix :) 

---

## 📝 Otra documentación...
- ✓ Regresar al README: [`README`](README.md)
- ✓ Código inicial: [`Versión 1`](./Codigo.md)
- ✓ Código actualizado: [`Versión 2`](./Codigo2.md)

