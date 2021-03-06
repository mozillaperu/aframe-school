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

## Extender con Entidad-Componente &mdash; Desde el Registro

> [El Registro](https://aframe.io/registry/) es un gran lugar para consegur componentes
> frescos que la comunidad ha agregado a A-Frame. Algo como complementos de
> terceros. Encuentra componentes de la comunidad desde el Registro, copia sus enlaces JS,
> inclúyelos con una etiqueta `<script>`, y úsalos directamente desde HTML.

1. Inclye el [Particle System](https://www.npmjs.com/package/aframe-particle-system-component). Adjunta
los `<a-entity>` con componentes `particle-system` configurados a `preset: default`
y `preset: snow` ¡Abre el Inspector para jugar con los valores!
2. Incluye [Animation](https://www.npmjs.com/package/aframe-animation-component). Adjunta la
animación a la esfera para hacer palpitar su escala configurando el componente `animation`
con `property: scale`, `loop: true`, y `to: 1.1 1.1 1.1`
3. Incluye [Outline Effect](https://www.npmjs.com/package/aframe-outline-effect). Ponlo en el
`<script>` y adjunta el componente `outline` a la escena

<a href="https://glitch.com/~aframe-school-registry" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="media/img/registryexample.gif">

<a href="https://aframe-school-registry.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element class="cta-button" -->

------

## Usar JavaScript

> Usa JavaScript y las API del DOM para modificar programáticamente la escena y sus
> entidades. A-Frame no sólo es HTML; A-Frame provee acceso a JavaScript,
> Las API de DOM, y three.js debajo de todo para un completo control. [Lee sobre cómo *Usar
> JavaScript y las APIs de DOM* con
> A-Frame](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="media/img/js.jpg">

Para ver los logs de JavaScript, podemos abrir la consola de desarrollo del navegador
haciendo clic derecho en la página, hacer clic en el *Inspector* o *Inspector de Elementos*, y luego
clic en la pestaña *Consola*. Cuando vemos la solución, podemos ver los resultados
a través de la consola del navegador.

---

## Usar JavaScript &mdash; Obteniendo las Entidades

> Usa
> [`document.querySelector()`](https://developer.mozilla.org/docs/Web/API/Document/querySelector)
> y
> [`document.querySelectorAll()`](https://developer.mozilla.org/docs/Web/API/Document/querySelectorAll)
> para obtener una referencia a la escena y sus entidades. [Lee sobre cómo consultar
> las entidades](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#getting-entities-by-querying-and-traversing).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Obtén una referencia al elemento `<a-scene>` usando `var sceneEl = document.querySelector('a-scene');`
2. Obtén una referencia a todos los elementos `<a-entity>` usando `sceneEl.querySelectorAll('a-entity');`
3. Obtén una referencia a la entidad de la caja usando `sceneEl.querySelector('#box');`
4. Obtén una referencia a las entidades de la esfera y el cilindro en una llamada a `.querySelectorAll()` usando un selector multielemento. Obtén una referencia a las entidades de la esfera y el cilindro en una llamada a `.querySelectorAll()` agregando y seleccionando clases HTML

<a href="https://aframe-school-js.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

---

## Usar JavaScript &mdash; Modificando Entidades

> Usa
> [`Entity.setAttribute()`](https://aframe.io/docs/0.5.0/core/entity.html#setattribute-attr-value-componentattrvalue)
> para modificar entidades después de obtener del ejercicio anterior. [Lee
> sobre cómo modificar
> entidades](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#modifying-an-entity).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remix Lesson on Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Cambia el componente `rotation` de la entidad de la caja
2. Cambia la propiedad `height` del componente `geometry` de la entidad del cilindro
3. Cambia la propiedad `metalness` del componente `material` de la entidad de la esfera

<a href="https://aframe-school-js.glitch.me/solution2.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

---

## Usar JavaScript &mdash; Creando Entidades

> Usa [`document.createElement()`](https://developer.mozilla.org/docs/Web/API/Document/createElement)
> para crear entidades, `.setAttribute()` para configurarlas, y `.appendChild()`
> para agregarlas a la escena.  [Lee sobre cómo crear
> entidades](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#creating-an-entity-with-createelement).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Un bucle `for` de JavaScript, crea y agrega 50 `<a-box>` elementos con
posiciones y escalas aleatorias (usa `Math.random()`)

<a href="https://aframe-school-js.glitch.me/solution3.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

---

## Usar JavaScript &mdash; Manejando Eventos

> Usa
> [`.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener)
> para registrar una función que será llamada cuando un evento sea emitido.
> Luego manualmente emite ese evento para que que la función se ejeute. Después
> podemos usar las escucha de eventos para cambiar la escena basada en las entradas de usuario u otras
> eventos. [Lee sobre los eventos y escuchas de eventos con
> A-Frame](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#events-and-event-listeners).

<a href="https://glitch.com/~aframe-school-js" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Registra una escucha de evento en la caja para escuchar al evento `foo`. En la
   función, cambia el color de la caja
2. Emite el evento `foo` con
[`Entity.emit()`](https://aframe.io/docs/0.5.0/core/entity.html#emit-name-detail-bubbles)
y el cambio de color de la caja

<a href="https://aframe-school-js.glitch.me/solution4.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

------

## Agregar Interacciones de Cursor Basadas en la Mirada &mdash; Agregar la Entidad Cursor

> Usa el [componente `cursor`](https://aframe.io/docs/0.5.0/components/cursor.html)
> basada en la mirada para proveer la posibilidad de interactuar con entidades
> (principalmente para smartphones). [Lee sobre cómo desarrollar una galería de
> imágenes 360&deg;](https://aframe.io/docs/0.5.0/guides/building-with-components.html).

<a href="https://glitch.com/~aframe-school-cursor" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

Esta lección tiene todos las escucha de eventos ya conectadas. Sólo necesitamos
agregar una entidad con el componente `cursor`, el cual provee aquellos eventos basados
en entradas de usuario. Ten en cuenta que estos eventos no son proporcionados por
el navegador, sino a través de A-Frame.

1. Agrega una entidad [`<a-camera>`](https://aframe.io/docs/0.5.0/components/camera.html).
   Anteriormente A-Frame estuvo proporcionando una cámara predeterminada
2. Agrga una entida [`<a-cursor>`](https://aframe.io/docs/0.5.0/components/cursor.html)
   como una entidad hijo dentro de la entidad de la cámara
3. Arrastra la cámara alrededor del click en los paneles en escritorio. En smartphones,
   mira fíjamente los paneles para lanzar los clicks (por esos son, basado en la mirada)

<img class="stretch" data-src="media/img/gaze.gif">

<a href="https://aframe-school-cursor.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button glitch" -->

---

## Agregar Interacciones de Cursor Basadas en la Mirada &mdash; Manejar Eventos

> Usa los eventos `click`, `mouseenter`, `mouseleave` proporcionados por el
> [componente `cursor`](https://aframe.io/docs/0.5.0/components/cursor.html) basado
> en la mirada para cambiar las propiedades de un objeto.

El código en Glitch  tendrá la estructura del proyecto preparada. Podemos agregar código
JavaScript dentro del componente `handle-events`, marcado por los comentarios de código.

<a href="https://glitch.com/~aframe-school-cursor-handler" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Adjunta nuestro `controller-event-handler` a los cubos. Podemos adjuntarlo a todo de una vez a través del mixin
2. Agrega una escucha de evento para cambiar el color de la caja con el evento `mouseenter`
3. Agrega una escucha de evento para restaurar el color de caja en el evento `mouseleave`

<img class="stretch" data-src="media/img/gazehandler.gif">

<a href="https://aframe-school-cursor-handler.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button glitch" -->

------

## Agregar Modelos 3D &mdash; Modelos glTF

> Los modelos 3D son como imágenes de  aplicaciones 3D y VR, aunque un poco más
> pesadas. Un modelo 3D es creado de antemano en un programa de modelado 3D como
> [Blender](https://www.blender.org/) y consta de vértices, texturas,
> materiales. Recomendamos usar [glTF](https://github.com/KhronosGroup/glTF), un
> nuevo formato de archivo 3D estándar adaptado para la web. glTF es como el
> JPG de los modelos 3D.

<a href="https://glitch.com/~aframe-school-gltf-model" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Agrega el archivo `https://cdn.aframe.io/test-models/models/virtualcity/VC.gltf` al
atributo `src` del elemento `<a-asset-item id="cityModel">` para precargar el modelo
2. Agrega `#cityModel` al atributo `src` del elemento `<a-gltf-model>` para establecer y agregar el modelo

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24275925/63067074-0ff0-11e7-9440-7c855b9ea0fd.png">

<a href="https://aframe-school-gltf-model.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

---

## Agregar Modelos 3D &mdash; Animaciones en el Modelo glTF

> Los modelos pueden venir con animaciones. El modelo proporcionado anteriormente tiene muchas animaciones
> de vehículos cruzando la ciudad. En el anterior Glitch, tenemos proporcionado un simple
> componente `play-all-model-animations` que podemos adjuntar a nuestro modelo para reproducir
> sus animaciones. Coninúa trabajando desde tu Glitch actual.

1. Inclute el componente `animation-mixer` a través de un `<script>` dentro de
`<head>` después del script de A-Frame. Este componente está actualmente en el Registro,
y puede que algún día se incluya con A-Frame. `https://unpkg.com/aframe-extras.animation-mixer@3.4.0/dist/aframe-extras.animation-mixer.js`
2. Adjunta el componente `animation-mixer` al `<a-gltf-model>` configurándolo
a través de un atributo `animation-mixer`. Por defecto, esto reproducirá todas
las animaciones del modelo a la vez.

<img class="stretch" data-src="media/img/gltf.gif">

<a href="https://aframe-school-gltf-model.glitch.me/solution2.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

---

## Agregar Modelos 3D &mdash; Subiendo Modelos 3D

> Si tienes un modelo propio, puede ser complicado subirlo a una CDN ya que
> esto consiste en múltiples archivos que se referencian los unos a otros. Así que la manera
> más fácil que hemos encontrado es ponerlos en un repositorio de GitHub, publica la rama
> master del repositorio a GitHub Pages, y usa `rawgit.com` para servirlos. Alternativamente,
> configura Amazon S3. Hay más por venir.

------

## Agregar Seguimiento de Controles &mdash; Agregar Controles de Mano

> El seguimiento de controles de mano provee inmersión and interactividad con
> controles de mano. En el siguiente Glitch, tenemos movimientos pre-grabados
> de controles de mano y botones con [A-Frame Motion
> Capture](https://github.com/dmarcos/aframe-motion-capture-components).
> Ahora sólo tenemos que agregar las manos y manejar los eventos de interacción.

<a href="https://glitch.com/~aframe-school-hand-controls" target="_blank">Remezclar la Lección en Glitch</a>  <!-- .element: class="cta-button glitch" -->

1. Encuentra `<a-entity id="left">` y agrega el [componente hand-controls](https://aframe.io/docs/0.5.0/components/hand-controls.html)
configurado para la mano izquierda (`hand-controls="left"`)
2. Encuentra `<a-entity id="right">` y agrega el componente hand-controls
confiurado para la mano derecha (`hand-controls="right"`)
3. Mira el resultado y observa las manos moviéndose con movimientos pre-grabados

<img class="stretch" data-src="media/img/trackedcontrols.gif">

<a href="https://aframe-school-hand-controls.glitch.me/solution.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

---

## Agregar Seguimiento de Controles &mdash; Agregar Interactividad

> Hay muchos componentes para agregar interactividad con controles de mano.
> [controller-cursor](https://github.com/bryik/aframe-controller-cursor-component),
> [aabb-collider +
> grab](https://github.com/aframevr/aframe/tree/master/examples/showcase/tracked-controls/components),
> [super-hands](https://github.com/wmurphyrd/aframe-super-hands-component). Para
> esta lección, usaremos controller-cursor que actúa como un puntero laser para
> cada mano. Continua desde tu anterior Glitch.

1. Agrega el componente `controller-cursor` a ambas manos
2. En el componente `controller-event-handler`, cambia el color de las cajas
cuando las manos pasen sobre cada una con el evento `mouseenter`, y restaura el color
con el evento `mouseleave`

<img class="stretch" data-src="media/img/trackedcontrols2.gif">

<a href="https://aframe-school-hand-controls.glitch.me/solution2.html" target="_blank">Ver el Resultado</a>  <!-- .element: class="cta-button" -->

------


<!-- Las lecciones terminan aquí. -->


## Felicitaciones!

Están graduados de la Escuela A-Frame y ahora tienen una licenciatura
no certificada en WebVR.

<img class="stretch" data-src="https://cdn.hackaday.io/images/4174761433219325627.png">

Revisa [la documentación](https://aframe.io/docs/) para más guías para convertirte
en un maestro.
