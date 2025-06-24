# 🛒 Wanted - E-commerce de Productos Usados

**Wanted** es una aplicación SPA desarrollada con **React** que permite comprar y vender productos usados. Ofrece funcionalidades modernas como navegación por categorías, carrito de compras con persistencia de estado, integración con **Firebase Firestore**, carga de productos, mensajes dinámicos y un diseño responsive atractivo.

---

## ✨ Características

- 🧭 Navegación mediante React Router (SPA)
- 🛍️ Vista de productos con detalle individual
- 🗃️ Filtro de productos por categorías
- ➕ Agregado de productos al carrito con validación de stock
- 💼 Checkout y generación de orden de compra
- 🧠 Gestión global del carrito con React Context
- 🔥 Firebase Firestore como base de datos para productos y órdenes
- 🧹 Manejo de errores y loaders con SweetAlert y componentes condicionales
- 📱 Diseño responsive con Bootstrap y estilos personalizados
- 🚧 Rutas protegidas para secciones "En construcción"

---

## 🛠️ Tecnologías utilizadas

- [React](https://reactjs.org/)
- [React Router DOM](https://reactrouter.com/)
- [Firebase Firestore](https://firebase.google.com/products/firestore)
- [Bootstrap 5](https://getbootstrap.com/)
- [SweetAlert2](https://sweetalert2.github.io/)
- [Vite](https://vitejs.dev/) como bundler

---

## 📁 Estructura del Proyecto

/src
│
├── components/
│ ├── NavBar.jsx
│ ├── Cart.jsx
│ ├── ItemListContainer.jsx
│ ├── ItemDetailContainer.jsx
│ ├── ItemCount.jsx
│ ├── Checkout.jsx
│ ├── Footer.jsx
│ ├── Error.jsx
│ └── UnderConstruction.jsx
│
├── context/
│ └── CartContext.jsx
│
├── mock/
│ └── products.js
│
├── service/
│ └── firebase.js
│
├── App.jsx
├── main.jsx
└── App.css

---

## 🚀 Instalación y uso

1. **Clonar el repositorio**

```bash
 git clone https://github.com/tu-usuario/wanted-ecommerce.git
 cd wanted-ecommerce

2. **Instalar dependencias**
`npm install`

3. **Configurar Firebase**
Crea un proyecto en Firebase.

Habilita Firestore.

Crea un archivo firebase.js dentro de /src/service con tu configuración:

// src/service/firebase.js
// Import the functions you need from the SDKs you need
import { initializeApp } from "firebase/app";
import { getFirestore } from "firebase/firestore";
// TODO: Add SDKs for Firebase products that you want to use
// https://firebase.google.com/docs/web/setup#available-libraries

// Your web app's Firebase configuration
const firebaseConfig = {
apiKey: "AIzaSyCdNffmkJ0iXEmw8kKN3flmzw5YN05W5Rg",
authDomain: "wanted-18798.firebaseapp.com",
projectId: "wanted-18798",
storageBucket: "wanted-18798.firebasestorage.app",
messagingSenderId: "369243761828",
appId: "1:369243761828:web:6bb483f7a902f05c108a31",
};

// Initialize Firebase
const app = initializeApp(firebaseConfig);

export const db = getFirestore(app);


4. **Iniciar el servidor de desarrollo**
`npm run dev`

🔁 Carga inicial de productos
Inicia la app (npm run dev)

Haz clic en "Subir datos a Firestore"

Los productos se cargarán automáticamente en la colección productosUsados.


## 🖼️ Vista previa

![Vista previa de la app](/public/home-preview.png)


## 🧪 Funcionalidades principales
Ruta	                     Descripción
/	                    Página principal con listado de productos
/category/:categoryId	Productos filtrados por categoría
/item/:itemId	        Detalle de un producto
/cart	                Carrito de compras con opción de checkout
/checkout	            Formulario de compra y resumen de orden
/en-construccion	    Página genérica para rutas no implementadas
/*	                    Página de error 404 personalizada

##  🧑‍💻 Autor
Oscar Vitasse
Portfolio: https://github.com/OscarDeveloper9
GitHub: https://github.com/OscarDeveloper9

##  📜 Licencia
Este proyecto está bajo la licencia MIT. Puedes usarlo libremente para fines educativos o comerciales.



```
