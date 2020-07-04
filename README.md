El poder de la Web está en su universalidad. El acceso de todas las personas independientemente de la discapacidad es un aspecto esencial.

# A11y

## Accesibilidad Web:
Es la práctica continua de asegurarnos que todo lo que creamos para la web se puede usar, interpretar y operar por una variedad de personas en una variedad de situaciones.

**a11y** numerónimo de accesibilidad (a ccessibilit(11) y )

### ¿Por qué accesibilidad?

- Para incluir a personas en situaciones de discapacidad. (20% del mundo)
- Para mejorar la usabilidad de nuestros proyectos.
- Porque en algunos lugares es la ley.
- Americans with Disabilities Act (ADA) became law in 1990.
- - Dominos pizza perdió un caso por esto [link](https://www.cnbc.com/2019/10/07/dominos-supreme-court.html)

El modo vibración no fue creado para reuniones, si no para personas que no pueden escuchar.


## ANDI
Can use ANDI (Accessible name & description inspector) is a free tool to test web content for accessibility.
- tabIndex
- aria-label

## WCAG
**Web Content Accessibility Guidelines** - *Pautas de Accesibilidad para el Contenido Web.*
Un rango de recomendaciones para crear contenido web más accesible.

### Historia de WCAG
- **W3C** *(World Wide Web Consortium):* Creadores de los estándares que usamos para construir la web.
- - **WAI** *(Web Accessibility Initiative):* Iniciativa dentro de W3C cuya meta es asegurar la accesibilidad web.
- - - **2.0**: [link](http://www.sidar.org/traducciones/wcag20/es/) [link](http://accesibilidadweb.dlsi.ua.es/?menu=criterios-2.0) 11 dic (2008) - Tiene 4 principios, segmentados en 12 criterios de conformidad, y cada criterio se divide en 3 niveles:
- - - - **A**: Accesibilidad básica, (25 criterios)
- - - - **AA**: Intermedia, (13 criterios)
- - - - **AAA**: Avanzado (23 criterios) (Servicios del gobierno, universidades o servicios esenciales de la vida cotidiana)
- - - **2.1** En junio de 2018

### WCAG 2.0

#### 4 Principios de WCAG
**Perceptible:** La información y los componentes de la interfaz de usuario deben ser presentados a los Usuarios de modo que ellos puedan percibirlos.

**Operable:** Los componentes de la interfaz de usuario y la navegación deben ser operables.

**Comprensible:** La información y el manejo de la interfaz de usuario deben ser comprensibles.

**Robusto:** El contenido debe ser suficientemente robusto como para ser interpretado de forma fiable por una amplia variedad de aplicaciones de usuario, incluyendo las ayudas técnicas.

#### 12 criterios de conformidad - Resumen:
1. Perceptible

Los criterios de conformidad bajo este principio se enfocan en asegurar que todo el contenido que es importante se pueda interpretar de varias maneras. Aqui nos queremos

- 1.1 Asegurar que estamos proporcionando alternativas textuales para todo contenido no textual.
- 1.2 Proporcionar alternativas para los medios tempodependientes (como videos o audios, queremos ofrecer opciones como subtítulos o guiones).
- 1.3 Crear contenido que se pueda presentar de diferentes formas sin perder información o estructura.
- 1.4 Facilitar a los usuarios ver y oír el contenido, incluyendo la separación entre el primer plano y el fondo

2. Operable

Cuando hablamos de ser operable, queremos asegurarnos que nuestro sitio es fácil de usar y navegar, que se puede navegar de diferentes maneras y con mouse y/o teclado

- 2.1 Proporcionar acceso a toda la funcionalidad mediante del teclado
- 2.2 Darle a las usuarias suficiente tiempo para leer y usar el contenido (tener esto en cuenta cuando hacemos time outs, comunicarlos y dar opciones para pedir más tiempo si es necesario)
- 2.3 Tener mucho cuidado de no usar elementos que brillan o se mueven muy rápido ya que pueden provocar ataques, espasmos o convulsiones
- 2.4 Asegurarnos que nuestros usuarios pueden navegar, encontrar contenido y determinar dónde se encuentran en nuestros sitios

3. Comprensible

Hacer que nuestro sitio web sea comprensible nos asegura que un rango de personas lo pueden usar desde la persona que vive con una discapacidad mental que necesita patrones comunes para saber cómo usar la web hasta la persona que va de carrera y necesita consultar algo rápido

- 3.1 Tener en cuenta los tamaños de texto y contraste de colores para que los textos resulten legibles y comprensibles
- 3.2 Hacer que las páginas web aparezcan y operen de manera predecible.
- 3.3 Dar instrucciones para evitar errores y oportunidades para corregirlos cuando ocurren

4. Robusto

Cuando hacemos productos que funcionan en muchos lados, abrimos las posibilidades que cualquier persona los use sin importar su ubicación, máquina, navegador y mucho más

- 4.1 Maximizar la compatibilidad con las aplicaciones de usuario actuales y futuras, incluyendo las tecnologías asistivas

### Tecnologías Asistivas
Principales
**Visuales**
-Lectores de pantallas
-Extensiones que manipulan el CSS.
**Motoras**
-Varilla bucal
-Switch

# Evaluar la accesibilidad de un sitio Web
## Pruebas automáticas
Chrome dev tools, tiene unas pruebas automáticas para páginas estáticas, que podemos realizar desde **Lighthouse**

## Pruebas con simuladores de discapacidades visuales
### Algunas discapacidades visuales:

- Visión borrosa
- Protanopia (Rojos principalmente los cambia a verdes)
- Deuteranopia (Ven los colores más amarillos de lo normal)
- Acromatopsia (Incapacidad de ver cualquier color)

Extensión de Chrome: **NoCoffe** Nos permite modificar el css del sitio, de acuerdo a multiples discapacidades visuales.
Chrome dev tools, también nos proporciona una herramienta, en los 3 puntitos, more tools, **rendering**, y al final de esta página podremos ver la sección de *emulate visión deficiences*

## Pruebas Manuales con teclado
El teclado es muy importante en la accesibilidad web porque las tecnologías asistivas tienden a conectarse con el teclado para darle a sus usuarios diferentes maneras de navegar cuando no tienen acceso a un mouse o un teclado como nosotros.

Para moverse en el teclado:
**Adelante:** Tab
**Atrás:** Shift + Tab
**click:** Enter


Los elementos que reciben foco de teclado son elementos interacctivos:

- **Enlaces:** nos llevan a otra página, son para la navegación.
- **Botones:** nos ayudan a interactuar con la página de alguna manera.
- **Formularios:** requieren nuestra interacción para llenar nuestros datos.

Los div no reciben foco porque son un elemento presentacional, no esperan ninguna interacción a menos de que tú lo programes.

## Pruebas manuales con lectores de pantalla
**Lectores de Pantalla:** Software que mapea las páginas que usamos y las lee en voz alta. Usan el `Accessibility` Tree (DevTools, Inpect -> Accessibility)
Algunas combinaciones muy usuales de lectores de pantalla y navegadores:
- NVDA - Mozilla Firefox
- JAWS - Internet Explorer
- VoiceOver - Safari
- ChromeVox - Google Chrome

## Pruebas manuales con voiceOver
- Prender (fn + command + f5)
- Apagar ()
- Avanzar adelante (control + option + derecha)
- Avanzar atrás (control + option + izquierda)
- Pausar (control)
- Entrar (Control + option + mayus + abajo)
- Salir (Control + option + mayus + arriba)

# Trucos para ser mas accessible

## ¿Qué es el HTML semántico y por qué es importante?
El HTML semántico nos ayuda con algunos aspectos de presentación y le agrega significado (interacciones, presentación) a nuestro contenido en el navegador.

Algunas ventajas:
- Posicionamiento en buscadores.
- Accesibilidad.
- Practicidad.
- Reusabilidad.

```html
<!-- Sin semántica -->
<div></div>
  <div><div></div></div>
<div></div>
<!-- Con semántica -->
<header></header>
  <article><img /></article>
<footer></footer>
```

### Tabindex:
Indica si su elemento puede ser enfocado, y si participa en la navegación secuencial del teclado.

Valores de Tabindex:

- **Valor negativo (-1):** El elemento debe ser enfocado, pero no debe de ser accesible a través de la navegación (por teclado). (oculto)
- **Valor positivo (>0):** Debe poder ser enfocado y su orden relativo es definido por el valor del atributo.
- **Valor de 0:** Debe ser enfocado y ser accesible a través de la navegación secuencial del teclado, pero su orden relativo es definido por convención de la plataforma (de la estructura del html).

Se combina usualmente con aria-hidden, para ocultar el elemento totalmente.

## (ARIA) ACCESSIBLE RICH INTERNET APPLICATIONS
Define cómo realizar contenido Web y aplicaciones Web (especialmente las desarrolladas con Ajax y JavaScript) más accesibles a personas con discapacidades. Son un conjunto de atributos especiales para accesibilidad que pueden añadirse a cualquier etiqueta, pero especialmente adaptado a HTML. Por ejemplo, ARIA posibilita puntos de navegación accesibles, widgets JavaScript, sugerencias en formularios y mensajes de error, actualizaciones en directo, y más..

Fue creado por la W3C (en la WAI), lo crearon para que podamos comunicar cambios especiales en nuestras aplicaciones.

### Atributos de ARIA en HTML:

### **Roles:**  Define el tipo general del objeto. (Como un artículo, una alerta, o un deslizador) `role=""`
Los roles le comunican al navegadores cuales son las interacciones que debería esperar y cómo se va a usar este objeto en nuestro proyecto. Se usan en situaciones muy especificas, es mejor depender del HTML semántico para comunicar los roles (Porque los nevegadores y lectores de pantalla, ya estan optimizados para entender la semántica).


### **Propiedades:** Comunican atributos que son esenciales para el comportamiento o significado de un elemento pero que suelen comunicar visualmente cómo iconos.  `aria-label="forward-button"`


### **Estados:** Estados de ARIA: Comunican estados y cambios de estados en elementos que se suelen comunicar visualmente. `aria-hidden="true"`


### [Más propiedades y estados](https://www.w3.org/WAI/PF/aria-1.1/states_and_properties)

#### **aria-live:**
Se utilizan para establecer la prioridad con la que el lector de pantalla debe tratar los cambios a la página  en vivo.

los valores posibles son:
- `off` (default)
- `polite` (No interrumpir lectura lector pantalla, notificación no muy importante)
- `assertive` (interrumpe la lectura del lector de pantalla para notificar algo muy importante).

## CSS Accessibilidad de un sitio web

### Contraste de color
En chrome, en los textos. Tenemos una herramienta muy potente que es al inspeccionar el color de un texto, le damos click al color. y nos mostrará el *Contrast ratio* (Contraste entre el fondo y el texto) nos sugiere una curva de colores que pueden cumplir este ratio (Arriba no cumplen, al medio cumplen AA, y los inferiores AAA), y si lo expandimos podemos ver si cumplimos los requerimientoss de WCAG (AA (4.5), o AAA (7.0))

### Iconos
Asi pensemos que todos los entienden, a veces muchos iconos no son universales. Entonces no está de más agregarles un `aria-label` o un texto descriptivo para identificarlos.

### Skip Links
Son enlaces de página internos que ayudan a la navegación por la página actual, en lugar de a páginas completamente nuevas.

### Estilos de foco y hover
Buscando crear una experiencia igual o parecida para personas que usen tecnologías asistivas, nos podemos apoyar en foco y hover. Usualmente tratamos de homologar los estilos en ambos.
También nos podemos ayudar bastante con la pseudo-clase CSS `:focus-within` la cual representa que un elemento  ha recibido el foco o que contiene un elemento que ha recibido el foco.
No olvidar que los outline también ayudan mucho

## Extender la acesibilidad usando JavaScript
`.focus()`
Conocer el código de una tecla en javascript [click aquí](http://keycode.info/)