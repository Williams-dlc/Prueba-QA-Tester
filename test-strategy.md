Al abrir el archive index.html se muestra un juego en el cual se descubrieron los siguientes errores.
1. el botón de “Ingresar el numero aleatorio” no realizaba ninguna acción.
Corrección
En el archivo index.html, en la sección de script, falto llamar la función “checkGuess” para que realizara la acción definida en esta función.
2. Si el número a adivinar no es el correcto, la respuesta era la palabra” Incorrecto” sobre un fondo verde. Por lo que se si la palabra era “incorrecto” este debe de ir sobre un fondo rojo.
Corrección
En la línea de código número 79 del archivo index.html, se debe de colocar el siguiente código.
lastResult.style.backgroundColor = 'black';
3. Si el número de intentos es mayor a 10, el usuario deberá de perder. Esto no pasa.
Corrección
En la línea de código número 46 especifica el número de intentos con la variable llamada “ATTEMPS” con el número 5. Se corrigió a número 10.
4. Si el número que se ingresa es mayor, este debe de lanzar el mensaje “INCORRECTO, EL NUMERO ES MAYOR”, el programa no lo hace. De igual manera si el numero es menor que el ingresado, este debe de lanzar el mensaje “INCORRECTO, EL NUMERO ES MENOR”

Corrección
En las líneas de código 81 y 83 no se especificó bien el mensaje que se debe de mostrar. Se Corrigió lo siguiente.
if(userGuess < randomNumber) {
        lowOrHi.textContent = 'El número es menor!';
      } else if(userGuess > randomNumber) {
        lowOrHi.textContent = 'El número es mayor!';

