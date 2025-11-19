APUNTES COMPLETOS DE HTML Y CSS
Basados en todos los PDFs, imágenes y enlaces proporcionados.
===========================================================
1. INTRODUCCIÓN A HTML
===========================================================
HTML (HyperText Markup Language) define la estructura de una página web.
Estructura básica:
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Mi página</title>
</head>
<body>
Contenido visible
</body>
</html>
Elementos principales:
- <html> raíz del documento.
- <head> metadatos, estilos, scripts.
- <body> contenido visual.
Semántica HTML:
header, nav, section, article, aside, footer
Se utilizan para mejorar accesibilidad y SEO.
Tipografías:
- Serif: con remates, elegantes.
- Sans-serif: limpias y legibles.
- Monospace: caracteres de ancho fijo.
Fuentes web:
@font-face permite cargar fuentes personalizadas.
===========================================================
2. FORMULARIOS HTML5
===========================================================
<form> contenedor.
<input> campos: text, email, password, number, date.
<select> listas desplegables.
<textarea> texto multi-línea.
Atributos:
placeholder: texto guía.
required: campo obligatorio.
autofocus: enfoca el campo al cargar la página.
min/max: límites numéricos.
fieldset y legend: agrupan campos.
Buenas prácticas:
- Etiquetas claras.
- Evitar abreviaturas.
- Usar descripciones cuando sea necesario.
- No abusar de placeholder.
===========================================================
3. CSS: FUNDAMENTOS
===========================================================
CSS controla la presentación de HTML.
Insertar CSS:
1. Inline: style="color:red"
2. Interno: <style>...</style>
3. Externo: <link rel="stylesheet" href="styles.css">
Selectores:
Simples:
p aplica a todos los párrafos
.clase por clase
#id por ID
Combinadores:
div p descendiente
div > p hijo directo
h1 + p hermano adyacente
div ~ p hermanos siguientes
Pseudoclases:
:hover ratón encima
:focus elemento enfocado
:active clic presionado
:first-child
:last-child
:nth-child(n)
Pseudoelementos:
::before
::after
::first-letter
::first-line
::selection
Selectores de atributo:
a[href$="pdf"] enlaces que terminan en pdf
===========================================================
4. BOX MODEL
===========================================================
Cada elemento es una caja formada por:
content + padding + border + margin
Propiedades:
padding: espacio interno
margin: espacio externo
border: borde
width/height: tamaño del contenido
box-sizing:
content-box (por defecto)
border-box (recomendado)
===========================================================
5. DISPLAY
===========================================================
block: ocupa la línea completa
inline: ocupa solo su contenido
inline-block: inline pero con dimensiones
none: desaparece del documento
visibility: hidden oculta pero mantiene el espacio
===========================================================
6. COLORES, FONDOS, SOMBRAS Y DEGRADADOS
===========================================================
color: color de texto.
background: fondo de un elemento.
background: url(img.jpg) no-repeat center/cover;
box-shadow:
box-shadow: 2px 2px 10px rgba(0,0,0,0.3);
text-shadow:
text-shadow: 1px 1px 3px #000;
Degradados:
background: linear-gradient(45deg, blue, red);
===========================================================
7. FLEXBOX (guía completa)
===========================================================
display: flex activa el modelo flex.
Ejes:
- Eje principal (horizontal por defecto).
- Eje secundario (vertical por defecto).
Propiedades del contenedor:
flex-direction: row | column | row-reverse | column-reverse
flex-wrap: nowrap | wrap | wrap-reverse
flex-flow: combinación de direction + wrap
justify-content: alineación horizontal
align-items: alineación vertical
align-content: alineación del conjunto
Propiedades de los hijos:
flex-grow: crecimiento del ítem
flex-shrink: reducción del ítem
flex-basis: tamaño base
flex: atajo grow shrink basis
order: orden visual
Ejemplo:
.container {
display: flex;
justify-content: center;
align-items: center;
}
===========================================================
8. CSS GRID (guía completa)
===========================================================
display: grid activa el modelo grid.
Columnas y filas:
grid-template-columns: 1fr 1fr 1fr
grid-template-rows: auto 200px
repeat():
grid-template-columns: repeat(3, 1fr)
fr = fracción del espacio disponible.
grid-gap o gap: separación
grid-area: sistema avanzado de zonas:
grid-template-areas:
"header header"
"menu main"
"footer footer"
Posicionamiento manual:
grid-column: 1 / 3
grid-row: 2 / 4
Funciones:
minmax(min, max)
auto-fit y auto-fill para grids dinámicos
===========================================================
9. RESPONSIVE DESIGN
===========================================================
viewport:
<meta name="viewport" content="width=device-width, initial-scale=1.0">
Media queries:
@media (max-width: 600px) {
body { background: red; }
}
Breakpoints recomendados:
600px móviles
768px tablet
992px portátil
1200px escritorio grande
vh/vw:
1vh = 1% alto del viewport
1vw = 1% ancho del viewport
===========================================================
10. DARK MODE AUTOMÁTICO
===========================================================
@media (prefers-color-scheme: dark) {
body {
background: black;
color: white;
}
}
===========================================================
11. VARIABLES CSS (CUSTOM PROPERTIES)
===========================================================
Definir variables:
:root {
--color-principal: blue;
}
Usarlas:
background: var(--color-principal);
Mejoran mantenibilidad y consistencia.
===========================================================
12. FLEX Y GRID POSTERS (síntesis de imágenes)
===========================================================
FLEXBOX:
justify-content:
- flex-start
- flex-end
- center
- space-between
- space-around
- space-evenly
align-items y align-content:
- flex-start
- flex-end
- center
- stretch
- baseline
GRID:
justify-items / align-items controlan items.
justify-content / align-content controlan grid entero.
grid-auto-flow:
row | column | dense | row dense | column dense
===========================================================
FIN DE LOS APUNTES COMPLETOS.
===========================================================