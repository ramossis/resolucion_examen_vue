# solucion_examen

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VS Code](https://code.visualstudio.com/) + [Vue (Official)](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

### Resolucion Examen VueJS SEM-2/26 INF-3911

## Parte Teorica

# Que es Vue js?

- Vue Js es un framework progresivo de JavaScript utilizado para construir interfaces de usuario y aplicaciones web de una sola pagina (SPA = Sigle Page Aplicaction) basado en arquitectura de componentes reactivos

# Que es reactividad?

- Es la capacidad de un framework que tiene para detectar automaticamente los cambios en el estado de los datos (**ref**,**reactive**) y actualizar de forma eficiente el DOM Document Object Model (la vista) sin necesidad de manipularlo manualmente

# De 2 ejemplos de frameworks basados en vue

- **Nuxt** = Metaframerok de Vue, tiene SSR , facil de manejar.
- **QUASAR** = Framework de Vue para desarollar apliaciones multiplataforma (Web, Escritorio , Movil)

# Para que sirve el atributo v-slot?

- Sirve para especificar a que ranura (slot) nombrada de un compoente hijo de debe enviar un bloque de contenido HTML desde el componente padre, asi como para recibir propiedades expuestas por el hijo (scoped slots) su abreviatura es #.

# De un ejemplo para el uso de eventos en emit

- Cuando un componente hijo (por ejemplo un boton o formulario) notifica una accion o envia datos al componente padre:
  - Hijo : emit('agregar-producto', producto)
  - Padre : <TarjetaProducto @agregar-producto="procesaCompra">

# Cuales son las formas de enviar parametros a una API?

- **Rouute Params/Path Paramas**:En la propia ruta URL (ej. /usuarios/15)
- **Query Params**: Mediante pares clave-valor despues de ? en la URL (ej. /usuarios?rol=admin&activo=true).
- **Body** (Cuerpo de la peticion): En formato JSON, FormData o x-www-form-urlenconded (usado en POST, PUT,PATCH).
- **Headers** (Cabeceras): Metadatos o tokens de autenticacion (ej. Autorization: Bearer <token>)

# Como se capturan los errores 404 en VueJs?

- En vue Router, definiendo una ruta comodin (catch-all) al final del arreglo de rutas mediante expresiones regulares:

````
  {
    path: '/:pathMatch(.*)*',
    name: 'NotFound',
    component: NotFoundView
  }
``
# Diferencia entre v-if y v-show
- v-if: Renderizado condicional real: crea o destruye el elemento en el DOM segun la condicion (tiene mayor costo al alternar frecuentemente, pero menor costo inicial si es falso).
- v-show : Siempre renderiza el elemento en el DOM y solo alterna su visibilidad mediante la propiedad CSS display:none (ideal para elementos que cambian de visibilidad muy seguido).

# Que hace router history (createWebHistory)?
- Configura el modo de navegacion utilizando la API History de HTML5 (history.pushState), permitiendo URLs limpias sin el simbolo # (hash) y sicronizando la navegacion con los botones de atras/adelante del navegador sin recargar la pagina
# Mencione 5 eventos que se pueden controlar con VueJS
## Recommended Browser Setup
- Chromium-based browsers (Chrome, Edge, Brave, etc.):
  - [Vue.js devtools](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)
  - [Turn on Custom Object Formatter in Chrome DevTools](http://bit.ly/object-formatters)
- Firefox:
  - [Vue.js devtools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/)
  - [Turn on Custom Object Formatter in Firefox DevTools](https://fxdx.dev/firefox-devtools-custom-object-formatters/)

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

## Project Setup

```sh
npm install
````

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```
