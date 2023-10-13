# Matrix

\*¿ que hemos echo?

let elemento: obtiene del index matrix un elemento y lo guarda. (ojo el elemento es un Canvas)

let ctx: se obtiene 2D de Canvasy se guarda en ctx, con 2D se pueden realziar dibujos en canvas

let with: nada simplemente se ajusta al tamaño, ancho del navegador.

let height lo mismo pero del alto.

elemento.width. Aquí se establece el ancho del canvas para q sea igual al ancho de la ventana del navegador.

elemento.height. Lo mismo pero del alto.

let position: Aquí se define el array sobre el que vana ir cayendo luego todos los simbolos, es importante poner de más porque va un poco en fn de la pantalla. si pones (5) veras solo 4 lineas de codigo. Poreso pongo 300 o 6000 de igual. Luego con .join se unen todos los elementos de la matriz y se devuelve la resultante. con .split simplente se separa la cadena con un "" entre cada uno

Funcion inicio

Antesde nada, let ctx será el elemento a pintar todo lo que vayamos a hacer sobre el elemento a pintar tiene que llevar ese nombre, si el nameing es horrible pero tiene que ser así.

- ctx.fillStyle Aquí se da el color de fondo, pero tiene una animación para darle una opacidad cuando se vaya la letra.
- ctx.fillRect con esto se va a dibujar un "rectangulo" que ocupará desde la izq a la derecha. El color de relleno que tomara es el anterior.
- ctx.fillStyle establece el color de los caracteres que se dibujarán en la matriz.
  -ctx.font, nada le das el tamaño que quieres a las letras y el tipo de letra.

position,map
Vamos a iterar sobre la matriz position, que es la que monta todo. y para cada posición y e index hará una serie de cosas, luego nos devolverá un nuevo array:

- text aqui se va a guardar el generar un caracter aleatorio.
- x calcula laposición horizontal para dibujar el caracter.
- Después tiene q dibujarse el caracter canvas (text) en la posición x e y. En esto: matrix.getContext("2d").fillText(text, x, y);

- se va a comprar y con index s i y es > que 100 se quedará en 0
  y sino y valdrá 15

- setinterval: se llama a la fn principal además se ponen los miliSegundos con los que se da la animación.
