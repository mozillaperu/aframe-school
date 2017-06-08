<!-- Título de la presentación. -->
<!-- .slide: data-background="media/img/aframe.jpg" -->

<div class="talk-title">
  <h1>Escuela A-Frame</h1>
  <h3>Un curso interactivo sobre WebVR</h3>
  <p class="talk-info">
    <b><a href="https://aframe.io">aframe.io</a></b>
  </p>
</div>

------

## Prólogo

<!-- .slide: data-background="media/img/aframe.jpg" -->

> Usando [Glitch](https://glitch.com), la Escuela te dará ejercicios
> paso a paso ¡Para ayudarte a saltar en [WebVR](https://webvr.rocks)! La Escuela tiene
> secciones yendo **&larr;** y **&rarr;** pero también subsecciones yendo **&uarr;** y
> **&darr;**:

<img class="stretch" data-src="media/img/navigation.jpg">

**Navegar &darr;**

---

### Recursos para tu Aventura

1. [Revisa la documentación y preguntas frecuentes](https://aframe.io/docs/)
2. [Obten ayuda de devotos en Slack](https://aframe.io/community/#slack)
3. [Haz preguntas en Stack Overflow](http://stackoverflow.com/questions/ask/?tags=aframe)
4. Si estás prescenciando un taller ¡Levanta tu mano si tienes una pregunta!

**Navegar &rarr;**


<!-- Las lecciones empiezan a continuación. -->


------

## Glitch &mdash; Introducción

> La Escuela usa [Glitch](https://glitch.com) como entorno de aprendizaje
> y desarrollo para A-Frame.

<img class="stretch" data-src="media/img/glitch.jpg">

- Glitch te permite programar en el navegador sin tener que configurar algo
- Glitch te permite **remezclar** proyectos para usar proyectos existentes de
  A-Frame existentes como punto de inicio
- Glitch publica instantáneamente y almacena tu sitio con una URL (p.ej.,
  `https://aframe.glitch.me`)
- Glitch actualiza tu sitio en vivo en cada cambio de código
- Glitch permite que varias personas programen al mismo tiempo

*Si estás interesado(a) en configurar un entorno de desarrollo local, sigue adelante &darr;*

---

## Glitch &mdash; Remezclando un Proyecto Existente

> Glitch te permite remezclar o hacer un fork de un proyecto existente y usarlo
> como base para tu nuevo proyecto. Antes de empezar, te recomendamos enlazar
> Glitch a una [cuenta de GitHub](https://github.com/). Después de remezclar,
> Glitch te dará un proyecto aleatorio y una URL, que puedes cambiar.

<img class="stretch" data-src="media/img/glitch2.jpg">

<a href="https://glitch.com/~aframe/" target="_blank">Remezclar A-Frame en Glitch para iniciar</a>  <!-- .element: class="cta-button glitch" -->

---

## Glitch &mdash; Editando el Código

> Una vez que has [remezclado A-Frame en Glitch](https://glitch.com/~aframe/),
> revisa en dónde editarás tu código. Asómate y mira que incluso puedes
> editar el código de servidor backend, subir assets, crear nuevos archivos, o
> ¡Invitar a otros a editar contigo!

<img class="stretch" data-src="media/img/glitch3.jpg">

---

## Glitch &mdash; Visualización del proyecto

> Después que te has asomado por el editor, mira el proyecto en vivo.

<img class="stretch" data-src="media/img/glitch4.jpg">

---

## Glitch &mdash; Exportando tu Proyecto

> En cualquier momento, si quieres descargar tu proyecto o exportarlo a Github
> mira el menú *Advanced Options*. La descargar te dará un archivo `.tgz` que
> puedes descomprimir. Para proyectos A-Frame, importa lo que está en la carpeta
> `public/`, e ignora todo el código del lado del servidor.

<img class="stretch" data-src="media/img/glitch5.jpg">

Si descargas un proyecto, puede
Que estés interesado(a) en configurar un entorno de desarrollo web en la siguiente
sección **&darr;**. Sino ¡Sigue adelante **&rarr;** para empezar con A-Frame!

---

## [Opcional] Configurar un Entorno de Desarrollo Web

> Puedes configurar un entorno de desarrollo web completo en un máquina locl, en
> lugar de usar el entorno de desarrollo en línea de Glitch.

<img class="stretch" data-src="media/img/webdevenv1.jpg">

1. **Obtener un editor de texto:** [Atom](https://atom.io) es uno bueno con
el cual empezar
2. **Configurar un servidor local:** Descarga y ejecuta [Mongoose
Server](https://www.cesanta.com/products/binary) o ejecuta `python -m
SimpleHTTPServer` en una terminal
3. **Crea un archivo `index.html`** y copia el código de A-Frame de los ejemplos
de Glitch
4. **Ejecuta un servidor local** en el mismo directorio en el que está el archivo
HTML
5. **Abre la URL del servidor local** en tu navegador (p.ej., `http://localhost:8000`)
6. **Haz cambios** a tu archivo HTML y refresca tu navegador para ver los cambios
7. Opcional: Revisa [ngrok](https://ngrok.io) para permitir que cualquier dispositivo
tenga acceso a tu servidor local

---

## [Opcional] Configurar un Entorno de Desarrollo Web &mdash; Obtener un Editor de Texto

> [Atom](https://atom.io) es un buen editor de texto para empezar si no tienes uno.
> Otra opciones populares son [Notepad++](https://notepad-plus-plus.org/),
> [Sublime](https://www.sublimetext.com/), [Brackets](http://brackets.io/), o
> [vim](http://www.vim.org/download.php).

<img class="stretch" data-src="media/img/webdevenv2.jpg">

---

## [Opcional] Configurar un Entorno de Desarrollo Web &mdash; Configurar un Servidor Local

> Necesitas un servidor HTTP local para servir tus archivos al navegador.

<div class="captioned-image-row small">
  <div>
    <img data-src="https://cloud.githubusercontent.com/assets/8731271/24021623/10654d22-0a5f-11e7-9769-63cdff91637c.png">
    <a href="https://www.cesanta.com/products/binary">Mongoose Binary</a>
  </div>
  <div>
    <img data-src="https://www.python.org/static/opengraph-icon-200x200.png">
    <code>python -m SimpleHTTPServer 8080</code>
  </div>
  <div>
    <img data-src="https://www.echosteg.com/images/blog/standard/nodejs_logo.png">
    <a href="https://docs.npmjs.com/getting-started/installing-node">Node + npm + live-server</a>
  </div>
</div>

---

## [Opcional] Configurar un Entorno de Desarrollo Web &mdash; Usar ngrok

> Opcionalmente, puedes usar [ngrok](https://ngrok.com/) para ayudar a desarrollar
> tu proyecto A-Frame en un smartphone sin tener que tener una IP local.

1. Descarga y descomprime [ngrok](https://ngrok.com/download/) en cualquier lugar
2. Ejecuta ngrok, proporcionandole el número de puerto de tu servidor local
(`./ngrok http 8080`)
3. En la terminal, ngrok te dará una URL con un montón de letras y números
(p.ej., `https://abcdef123456.ngrok.io`)
4. Abre esa URL en otro dispositivo en cualquier red (como un smartphone u otra computadora)

<img class="stretch" data-src="media/img/webdevenv3.jpg">

------

## Probar los Ejemplos de A-Frame

> Juega con los ejemplos en tu escritorio o smartphone desde la [página de
> A-Frame](https://aframe.io), [el Blog de A-Frame](https://aframe.io/blog/), o
> [awesome-aframe](https://github.com/aframevr/awesome-aframe). Mira
> [webvr.rocks](https://webvr.rocks) para información o configurar WebVR con un
> visor si tienes uno.

<img data-src="media/img/examples.gif">

------

## Empezar con *Hola, WebVR*

> A-Frame provee elementos HTML fáciles de usar para principiantes llamados
[primitives](https://aframe.io/docs/0.5.0/primitives/). En las siguientes secciones,
modificaremos los cosas básicas a través de atributos HTML (p.ej., cambiar colores,
posiciones, rotaciones, escala) y tener una idea del flujo de trabajo.

<img data-src="media/img/hellowebvr2.jpg">

<img class="stretch" data-src="media/img/hellowebvr.jpg">

---

## Empezar con *Hola, WebVR* &mdash; Posición

> La posición define en dónde están los objetos en el espacio 3D (X, Y, Z) en metros.
> Cambia la `posición` de los objetos a traves los valores del atributo HTML `position`.
> [Lee sobre posiciones](https://aframe.io/docs/master/components/position.html).

<a href="https://glitch.com/~aframe-school-position" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Mover el cilindro hacia la izquierda *reduciendo* el valor X de `position`
2. Mueve la caja hacia arriba *aumentando* el valor Y de `position`
3. Mueve la esfera hacia atrás *reduciendo* el valor Z de `position`
4. **Crédito adicional:** Agregar `<a-ring>` dentro de `<a-sphere>` y dale una
posición para ver las posiciones relativas

<img class="stretch" data-src="media/img/positionresult.jpg">

<a href="https://aframe-school-position.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

---

## Empezar con *Hola, WebVR* &mdash; Rotación

> La rotación define la orientación de los objetos en el espacio 3D (sobre lo ejes
> X, Y, Z) een grados. Usa regla de la derecha para visualizar parcialmente
> la rotación. [Lee sobre rotaciones](https://aframe.io/docs/master/components/rotation.html).

<a href="https://glitch.com/~aframe-school-rotation" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Gira el cilindro al rededor del eje X para ver el fondo
2. Gira la caja al rededor del eje Y para que la caja esté mirando hacia arriba
3. **Crédito adicional:** Envuelve el contenido de la escena con `<a-entity>`
(como un `<div>`) y date una rotación para ver las rotaciones relativas

<img class="stretch" data-src="media/img/rotationresult.jpg">

<a href="https://aframe-school-rotation.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

---

## Empezar con *Hola, WebVR* &mdash; Agregar Primitivos

> Agregar primitivos a la escena agregando elementos HTML debajo de `<a-scene>`-
> [Lee sobre primitivos](https://aframe.io/docs/0.5.0/primitives/).

<a href="https://glitch.com/~aframe-school-primitives" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Agrega [`<a-torus-knot>`](https://aframe.io/docs/0.5.0/primitives/a-torus-knot.html) a la izquierda
2. Agrega [`<a-dodecahedron>`](https://aframe.io/docs/0.5.0/primitives/a-dodecahedron.html) a la derecha
3. Agrega [`<a-text>`](https://aframe.io/docs/0.5.0/primitives/a-text.html) alineado en el centro

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24266010/9c57cbe4-0fc2-11e7-968f-168f3649d109.png">

<a href="https://aframe-school-primitives.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

------

## Agregar Texturas &mdash; Subiendo Recursos

> Agregaremos texturas de imagen para combinar para más apariencia que un color plano.
> [Encuentra tus propias imágnes
> en línea](https://aframe.io/docs/0.5.0/introduction/faq.html#where-can-i-find-assets),
> y súbelas a través de la sección de recursos en Glitch o a través del cargador en
> [cdn.aframe.io](https://cdn.aframe.io). En donde sea que subas, asegúrate
> que está siendo servidos con
> [CORS](https://developer.mozilla.org/docs/Web/HTTP/Access_control_CORS) y
> sobre HTTPS.

<img class="stretch" data-src="media/img/glitchasset.jpg">

En el siguiente Glitch **&darr;**, algunos recursos ya estarán disponibles en la
sección de recursos (imagen arriba).

---

## Agregar Texturas &mdash; Texturas de imagen

> Llena los atributos HTML `src` con las URL de las imágenes. [Lee sobre cómo aplicar
> una textura de imagen](https://aframe.io/docs/0.5.0/guides/building-a-basic-scene.html#applying-an-image-texture).

<a href="https://glitch.com/~aframe-school-textures/" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Agregar una textura de imagen al suelo, `<a-plane>`
2. Agrega texturas de imagen a las cajas, `<a-box>`
3. Agrega una textura de imagen a la esfera, `<a-sphere>`
4. Agrega una textura de imagen al cono, `<a-cone>`
5. Agrega una textura de imagen al fondo, `<a-sky>`. Encuentra [Imágenes de 360&deg; desde FLickr](https://www.flickr.com/groups/equirectangular/)

<img class="stretch" data-src="media/img/texture.jpg">

<a href="https://aframe-school-textures.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

------

## Abrir el Inspector de A-Frame

> Presiona **`<ctrl> + <alt> + i`** en **cualquier** escena A-Frame para abrir un editor
> visual ¡Como las Herramientas de Desarrollador de tu navegador! Prueba el Inspector en algunos
> de los [ejemplos de la página principal](https://aframe.io/examples/). [Lee sobre el
> Inspector](https://aframe.io/docs/master/guides/using-the-aframe-inspector.html).

<img class="stretch" data-src="media/img/inspector.gif">

---

## Abrir el Inspector de A-Frame &mdash; Cambiar Valores de Componentes

> Modifica una entidad cambiando sus componentes en el panel de la derecha. El
> Inspector sabe sobre todos los componentes de A-Frame, incluyendo los componentes de la comunidad.
> Este ejemplo incluye un [componente
> `text-geometry`](https://www.npmjs.com/package/aframe-text-geometry-component) externo, que
> el Inspector puede modificar los valores en vivo.

<a href="https://aframe-vaporwave.glitch.me" target="_blank">Abre el Ejemplo en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Selecciona una de las entidades con texto en el ejemplo
2. Cambia la propiedad `value` del [componente `text-geometry`](https://www.npmjs.com/package/aframe-text-geometry-component)

<img class="stretch" data-src="media/img/inspectorchange.jpg">

---

## Abrir el Inspector de A-Frame &mdash; Adjunta Componentes desde el Registro

> Usa [componentes de física](https://github.com/donmccurdy/aframe-physics-system)
> del [Registro](https://aframe.io/registry/) para agregar gravedad y colisiones.
> El Registro es una colección limpia de componeentes de A-Frame. Y el Inspector
> está enganchado al Registro, así que podemos agregar componentes desde el Registro en
> el panel de entidad.

<a href="https://aframe-vaporwave.glitch.me" target="_blank">Abre el Ejemplo en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Agrega el componente `static-body` a la grilla del piso
2. Agrega el componente `dynamic-body` al nudo del toro (la rosca púrpura de atrás)
3. Incrementa la posición Y del nudo del toro para hacerlo más alto
4. Salir del Inspector

<img class="stretch" data-src="media/img/inspectorregistry.gif">

------

## Componer con Entidad-Componente &mdash; Descomponer Primitivos

> Detrás de los elementos fáciles de usar, A-Frame está basado en una
> arquitectura entidad-componente. Descomponer los elementos primitivos en el
> ejemplo *Hello, WebVR* a elementos `<a-entity>` con sus componentes fundamentales.

<a href="https://glitch.com/~aframe-school-ecs" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

[geometry]: https://aframe.io/docs/0.5.0/components/geometry.html
[material]: https://aframe.io/docs/0.5.0/components/material.html

1. Convierte `<a-box>` a `<a-entity>` con el [componente geometry][geometry] y el [componente material][material]. Configura el componente geometry para que sea `primitive: box`
2. Convierte `<a-sphere>` a `<a-entity>` con los componentes geometry y material. Configura el componeente geometry para que sea `primitive: sphere`
3. Convierte `<a-cylinder>` a `<a-entity>` con los componentes geometry y material. Configura el componente geometry para que sea `primitive: cylinder`
4. Convierte `<a-plane>` a `<a-entity>` con los componentes geometry y material. Configura el componente geometry para que sea `primitive: plane`
5. Convierte `<a-sky>` a `<a-entity>` con los componentes geometry y material. Configura el componente geometry para que sea `primitive: sphere` con un gran `radius: 3000`, y configura el componente material para que sea `shader: flat` así no necesitamos hacer cálculos pesados para la luz cuando sólo necesitamos un color plano

<a href="https://aframe-school-ecs.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

---

## Componer con Entidad-Componente &mdash; Agregar una Esfera de Fuente de Luz

> Usa el patrón entidad-componente para agregar una esfera que también actúe como un punto
> de fuente de luz. Mezcla juntos los componente, geometry, material, y luz para
> componer este tipo de objeto.

1. Busca `<a-entity id="lightSphere">`
2. Adjunta el [componente geometry](https://aframe.io/docs/0.5.0/components/geometry.html) configurado para usar `primitive: sphere` a la entidad
3. Adjunta el [componente material](https://aframe.io/docs/0.5.0/components/material.html) configurado para usar `color: #FFF` y `shader: flat` a la entidad
4. Adjunta el [componente light](https://aframe.io/docs/0.5.0/components/light.html) configurado para usar `type: point` a la entidad
5. **Crédito adicional:** Agrega el componente animation del [Registro](https://aframe.io/registry/) a través de la etiqueta `<script>`. Adjunta la animación configurada para usar `property: position` y `dir: alternate` y `loop: true` y proporcionar un valor de posición para `to: <POSITION>`

<a href="https://glitch.com/~aframe-school-ecs-light-sphere" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24060160/2c53a604-0b0f-11e7-9386-f83a3a9b4cfc.gif">>

<a href="https://aframe-school-ecs-light-sphere.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element class="cta-button" -->

------

## Extend with Entity-Component &mdash; From the Registry

> [The Registry](https://aframe.io/registry/) is a great place to grab cool
> components that the community has added to A-Frame. Sort of like third-party
> plugins. Find community components from the Registry, copy their JS links,
> include them via a `<script>` tag, and use them straight from HTML.

1. Include [Particle
System](https://www.npmjs.com/package/aframe-particle-system-component). Attach
`<a-entity>`s with `particle-system` components configured to `preset: default`
and `preset: snow`. Open the Inspector to play with the values!
2. Include [Animation](https://www.npmjs.com/package/aframe-animation-component). Attach
animation to the sphere to throb its scale by configuring `animation` component
with `property: scale`, `loop: true`, and `to: 1.1 1.1 1.1`
3. Include [Outline Effect](https://www.npmjs.com/package/aframe-outline-effect). Drop in the
`<script>` and attach the `outline` component to the scene

<a href="https://glitch.com/~aframe-school-registry" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="media/img/registryexample.gif">

<a href="https://aframe-school-registry.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element class="cta-button" -->

------

## Use JavaScript

> Use JavaScript and DOM APIs to programmatically modify the scene and its
> entities. A-Frame is not just HTML; A-Frame provides access to JavaScript,
> DOM APIs, and three.js underneath for full control.  [Read about *Using
> JavaScript and DOM APIs* with
> A-Frame](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="media/img/js.jpg">

To see JavaScript logs, we can open the browser's development console by
right-clicking the page, clicking *Inspect* or *Inspect Element*, and then
clicking the *Console* tab. When viewing solutions, we can see the results
through the browser console.

---

## Use JavaScript &mdash; Getting Entities

> Use
> [`document.querySelector()`](https://developer.mozilla.org/docs/Web/API/Document/querySelector)
> and
> [`document.querySelectorAll()`](https://developer.mozilla.org/docs/Web/API/Document/querySelectorAll)
> to get a reference to the scene and its entities.  [Read about querying for
> entities](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#getting-entities-by-querying-and-traversing).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Get a reference to the `<a-scene>` element using `var sceneEl = document.querySelector('a-scene');`
2. Get a reference to all `<a-entity>` elements using `sceneEl.querySelectorAll('a-entity');`
3. Get a reference to the box entity using `sceneEl.querySelector('#box');`
4. Get a reference to the sphere and cylinder entities in one `.querySelectorAll()` call by using multi-element selector
. Get a reference to the sphere and cylinder entities in one `.querySelectorAll()` call by adding and selecting HTML classes

<a href="https://aframe-school-js.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Use JavaScript &mdash; Modifying Entities

> Use
> [`Entity.setAttribute()`](https://aframe.io/docs/0.5.0/core/entity.html#setattribute-attr-value-componentattrvalue)
> to modify entities after retrieving them from the previous exercise. [Read
> about modifying
> entities](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#modifying-an-entity).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Change the box entity's `rotation` component
2. Change the cylinder entity's `geometry` component's `height` property
3. Change the sphere entity's `material` component's `metalness` property

<a href="https://aframe-school-js.glitch.me/solution2.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Use JavaScript &mdash; Creating Entities

> Use [`document.createElement()`](https://developer.mozilla.org/docs/Web/API/Document/createElement)
> to create entities, `.setAttribute()` to configure them, and `.appendChild()`
> to add them to the scene.  [Read about creating
> entities](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#creating-an-entity-with-createelement).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. In a JavaScript `for` loop, create and add 50 `<a-box>` elements with
random positions and scales (use `Math.random()`)

<a href="https://aframe-school-js.glitch.me/solution3.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Use JavaScript &mdash; Handling Events

> Use
> [`.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener)
> to register a handler function that will be called when an event is emitted.
> Then manually emit that event to see that handler function execute. Later we
> can use event listeners to change the scene based on user input or other
> events. [Read about events and event listeners with
> A-Frame](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#events-and-event-listeners).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Register an event listener on the box to listen to the `foo` event. In the
   handler function, change the box's color
2. Emit the `foo` event with
[`Entity.emit()`](https://aframe.io/docs/0.5.0/core/entity.html#emit-name-detail-bubbles)
and see the box change its color

<a href="https://aframe-school-js.glitch.me/solution4.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

------

## Add Gaze-Based Cursor Interactions &mdash; Add Cursor Entity

> Use the gaze-based [`cursor`
> component](https://aframe.io/docs/0.5.0/components/cursor.html) to provide
> the ability to interact with entities (primarily for smartphones).  [Read
> about building a 360&deg; image
> gallery](https://aframe.io/docs/0.5.0/guides/building-with-components.html).

<a href="https://glitch.com/~aframe-school-cursor" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

This lesson has all the event listeners hooked up already. We just need to add
an entity with the `cursor` component which will provide those events based on
user input.  Note these events are not provided by the browser, but through
A-Frame.

1. Add [`<a-camera>`](https://aframe.io/docs/0.5.0/components/camera.html) entity.
   Previously A-Frame was providing a default camera
2. Add [`<a-cursor>`](https://aframe.io/docs/0.5.0/components/cursor.html) entity
   as a child underneath the camera entity
3. Drag the camera around the click on the panels on desktop. On smartphones,
   stare at the panels to trigger clicks (i.e., gaze-based)

<img class="stretch" data-src="media/img/gaze.gif">

<a href="https://aframe-school-cursor.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button glitch" -->

---

## Add Gaze-Based Cursor Interactions &mdash; Handle Events

> Use the `click`, `mouseenter`, `mouseleave` events provided by the gaze-based
> [`cursor` component](https://aframe.io/docs/0.5.0/components/cursor.html) to
> change the properties of an object.

The Glitch code will have the project structure set up. We can add JavaScript
code inside the `handle-events` component, marked by the code comments.

<a href="https://glitch.com/~aframe-school-cursor-handler" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Attach our `controller-event-handler` to the cubes. We can attach to all of them at once through the mixin
2. Add an event listener to change the box's color on `mouseenter` event
3. Add an event listener to restore the box's color on `mouseleave` event

<img class="stretch" data-src="media/img/gazehandler.gif">

<a href="https://aframe-school-cursor-handler.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button glitch" -->

------

## Add 3D Models &mdash; glTF Model

> 3D models are like the images of 3D and VR applications, although a bit
> heavier. A 3D model is created beforehand in a 3D modeling program such as
> [Blender](https://www.blender.org/) and consists of vertices, textures,
> materials. We recommend using [glTF](https://github.com/KhronosGroup/glTF), a
> relatively new 3D file format standard tailored for the Web. glTF is like the
> JPG of 3D models.

<a href="https://glitch.com/~aframe-school-gltf-model" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Add the `https://cdn.aframe.io/test-models/models/virtualcity/VC.gltf` to
the `<a-asset-item id="cityModel">`'s `src` attribute to preload the model
2. Add `#cityModel` to the `<a-gltf-model>`'s `src` attribute to set and add the model

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24275925/63067074-0ff0-11e7-9440-7c855b9ea0fd.png">

<a href="https://aframe-school-gltf-model.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Add 3D Models &mdash; glTF Model Animations

> Models can come with animations. The model provided above has many animations
> of ships zooming across the city. In the previous Glitch, we've provided a simple
> `play-all-model-animations` component that we can attach to our model to play
> its animations. Continue working from your current Glitch.

1. Include the `animation-mixer` component via a `<script>` in the
`<head>` after the A-Frame script. This component is currently in the Registry,
and may one day be included with A-Frame. `https://unpkg.com/aframe-extras.animation-mixer@3.4.0/dist/aframe-extras.animation-mixer.js`
2. Attach the `animation-mixer` component to the `<a-gltf-model>` by
setting it via an HTML attribute `animation-mixer`. By default, this will play all
the animations of the model at once.

<img class="stretch" data-src="media/img/gltf.gif">

<a href="https://aframe-school-gltf-model.glitch.me/solution2.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Add 3D Models &mdash; Uploading 3D Models

> If you have a model of your own, it can be tricky to upload it to a CDN since
> it consists of multiple files that reference each other. So far the easiest
> way we've found is to dump them into a GitHub repo, publish the repo's master
> branch to GitHub Pages, and use `rawgit.com` to serve them. Alternatively,
> set up Amazon S3. More to come.

------

## Add Tracked Controls &mdash; Add Hand Controls

> Tracked hand controls provide immersion and interactivity with hand
> controllers. In the following Glitch, we've pre-recorded hand control
> movements and button presses with [A-Frame Motion
> Capture](https://github.com/dmarcos/aframe-motion-capture-components).
> Now we just have to add the hands and handle the interaction events.

<a href="https://glitch.com/~aframe-school-hand-controls" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Find `<a-entity id="left">` and add the [hand-controls component](https://aframe.io/docs/0.5.0/components/hand-controls.html)
configured to the left hand (`hand-controls="left"`)
2. Find `<a-entity id="right">` and add the hand-controls component
configured to the right hand (`hand-controls="right"`)
3. View the result and see the hands moving with pre-recorded motions

<img class="stretch" data-src="media/img/trackedcontrols.gif">

<a href="https://aframe-school-hand-controls.glitch.me/solution.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

---

## Add Tracked Controls &mdash; Add Interactivity

> There are many components to add interactivity to hand controls.
> [controller-cursor](https://github.com/bryik/aframe-controller-cursor-component),
> [aabb-collider +
> grab](https://github.com/aframevr/aframe/tree/master/examples/showcase/tracked-controls/components),
> [super-hands](https://github.com/wmurphyrd/aframe-super-hands-component). For
> this lesson, we'll use controller-cursor that acts as a pointing laser for
> each hand. Continue from your previous Glitch.

1. Add `controller-cursor` component to both hands
2. In the `controller-event-handler` component, change the color of the boxes
when they are hovered over with the `mouseenter` event, and restore the color
with the `mouseleave` event

<img class="stretch" data-src="media/img/trackedcontrols2.gif">

<a href="https://aframe-school-hand-controls.glitch.me/solution2.html" target="_blank">View Result</a>  <!-- .element: class="cta-button" -->

------


<!-- Lessons end here. -->


## Congratulations!

You've graduated from the A-Frame School and now have a virtual uncertified
degree in WebVR.

<img class="stretch" data-src="https://cdn.hackaday.io/images/4174761433219325627.png">

Head to [the documentation](https://aframe.io/docs/) for more guides to become
a master.
