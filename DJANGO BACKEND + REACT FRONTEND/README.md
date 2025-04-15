# 🚀 Creación del Proyecto

Este proyecto es una aplicación web que combina un backend en **Django** y un frontend en **React**. A continuación, te guiaremos paso a paso para configurarlo desde cero.

## Prerrequisitos
- Python 3.x instalado
- Node.js y npm instalados
- Conocimientos básicos de terminal y comandos
- Un editor de código (recomendado: VS Code)

## 1 - Generamos el Backend

```bash
django-admin startproject backend
```

## 2 - Generamos el Frontend

```bash
npx create-react-app frontend
```

## 3 - Visualizar la interfaz inicial

- Entramos al proyecto generado del frontend:
```bash
cd frontend
```

- Desplegamos el proyecto para poder visualizar su interfaz desde la web:
```bash
npm start
```

- En este punto no es necesario resetear el ```npm start``` debido a que react actualiza de forma automatica la visualización.

## 4 - Creación de la interfaz inicial

- Para este paso nos dirigimos a **src** y buscamos el archivo **App.js** en el cual ya vemos que tiene la interfaz inicial por defecto.

- Para modificar la interfaz, tomamos en cuenta en que consiste el proyecto y que herramientas de react de interfaz vamos a usar, como en este caso usamos el manejo de rutas por la razon de que nos movilizaremos en la web, pararemos con **ctrl** + **c**, e instalaremos la siguiente dependencia:
```bash
npm install react-router-dom
```

- Ahora que tenemos la **route** de react, agregaremos en nuestro **App.js** la siguiente importación:
```js
import { BrowserRouter as Router, Routes, Route } from 'react-router-dom';
```

- Ahora podremos volver a correr el proyecto sin errores y solo una advertencia (Esta advertencia se debe a que el App.js no esta usando el **Route**) corremos poniendo:
```bash
npm start
```

- Ahora crearemos lo que sería nuestro **navbar** inicial, el cual llevara un menu de opciones para la fase donde los usuarios no estan registrados.
- - Para este paso, en la carpeta **src** agregaremos la carpeta **components** y crearemos el archivo **Navbar.jsx** junto a lo que seria su hoja de estilos **Navbar.css**

- Creación del **Navbar.jsx**

- - Dentro del **Navbar.jsx** importamos su hoja de estilo:
```js
import './Navbar.css';
```
- - Ahora creamos lo que sería su función, la cual contendra el contenido del navbar que se mostrara:
```js
function Navbar() {}
```

- - Como tal, definir a función, no muesta nada aún, por lo que dentro de la funcion del **Navbar** retornaremos lo que veremos en nuestra web:
```js
function Navbar() {
    return ();
}
```

- - Con **return** ya definido, podremos meter los componentes a mostrar los cuales son similares a las etiquetas de un **HTML**:
```js
<nav className="navbar">
</nav>
```