![react logo](https://xabikos.gallerycdn.vsassets.io/extensions/xabikos/reactsnippets/1.2.1/1486301381125/Microsoft.VisualStudio.Services.Icons.Default)

# React Workshop

## Tabla de Contenidos

### - [Introducción](#introduccion)

### - Teoría 

1. [React](#react)

2. [Virtual DOM](#virtual-dom)

3. [JSX](#jsx)

4. [Create React App](#create-react-app)

### - Práctica

1. React Components
    1. [React.Component](https://facebook.github.io/react/docs/react-component.html)
    2. [State & Props](https://facebook.github.io/react/docs/react-component.html#instance-properties)
    3. [Lifecycle](https://facebook.github.io/react/docs/react-component.html#the-component-lifecycle)
    4. [Events](https://facebook.github.io/react/docs/handling-events.html)

2. React Router

---

## Introducción 

Bienvenidos al Workshop de React!.

Este Workshop tiene como objetivo introducirlos en el mundo de ReactJS, vamos a estar dando una breve intro sobre ReactJS y después abordaremos a los correspondientes ejercicios.

### Prequisitos

- Fundamentos de ECMAScript 6 <https://www.acamica.com/cursos/134/es6-inicial>
- Introducción a React <https://www.acamica.com/cursos/119/introduccion-a-react>

### React 

React es una libreria de Javascript (open source) echa por Facebook en el año 2013. Desde ese entonces fue ganando popularidad y hoy en día esta en el top de librerias/frameworks (Backbone, Angular 1 y 2, Ember ...).

React es realmente útil para la creacion de *Interfaces de usuario* (*UI*) y se puede combinar con frameworks como Backbone para proveer una completa experiencia, ya que es solo una _VIEW LAYER_. 
Se puede usar para crear páginas simples que contengan botones o formularios, o largas y complejas vistas para envolver toda una aplicacion entera.

- [ReactJS Official web ]((https://facebook.github.io/react/))

### Virtual DOM

El secreto de ReactJS para tener un performance muy alto, es que implementa algo llamado "Virtual DOM" y en vez de renderizar todo el DOM en cada cambio, que es lo que normalmente se hace, este hace los cambios en una copia en memoria y después usa un algoritmo para comparar las propiedades de la copia en memoria con las de la versión del DOM y así aplicar cambios exclusivamente en las partes que varían.

Esto puede sonar como mucho trabajo, pero en la práctica es mucho más eficiente que el método tradicional pues si tenemos una lista de dos mil elementos en la interfaz y ocurren diez cambios, es más eficiente aplicar diez cambios, ubicar los componentes que tuvieron un cambio en sus propiedades y renderizar estos diez elementos, que aplicar diez cambios y renderizar dos mil elementos.

### JSX

React nos ofrece un pseudolenguaje llamado JSX que facilita el desarrollo de aplicaciones web con su sintaxis para crear elementos en el DOM.
Recordemos que ReactJS se enfoca en la visualización y literalmente debemos armar el HTML que deseamos directamente en JSX, con el fin de describir nuestros componentes por medio de etiquetas y de una sintaxis muy parecida a la de HTML, que es compilada a Javascript.
