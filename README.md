# quiz_millionaire
Práctica con elementos del DOM y javascript

En esta práctica tenemos sólo dos páginas html, la primera, de inicio, con un título y un botón que redirige al quiz.


Dentro del quiz, se lanzará automáticamente la música de tension de "50x15", cada pregunta se refresca al presionar el botón "Siguiente", 
es necesario elegir una de las opciones para que sea posible avanzar a través de el. Hay cuatro opciones posibles y sólo una es la correcta.

Si la respuesta es correcta, sumará un punto al "score", que se presenta al final del quiz.

Al completar las 10 preguntas, saltará la última pantalla con la puntuación final, y dependiendo de ella, un mensaje u otro.
De igual forma, si se saca menos de un 5, se repoducirá una música, y si se saca más, otra distinta.

A nivel de código, se encuentran en primer lugar los selectores de los elementos que actuarán en el proyecto, después
un array con los elementos de cada pregunta así como la respuesta correcta de cada una de ellas.

A continuación se declaran las variables de pregunta actual y puntuación, que irán cambiando según avance el quiz.

Por último se definen las funciones que harán que el quiz cobre vida:

- La función "loadQuiz" inicializa cada pregunta y sus respuestas, junto con "deselectAns" que declara las respuestas que
no han sido seleccionadas por el jugador.

- La función getSelected hace justo lo opuesto y marca la que sí ha sido seleccionada, la compara con la respuesta correcta y si coincide
se añade un punto al "score". Con el condicional dentro de la función hacemos que el quiz vaya avanzando hasta que la pregunta actual sea mayo que el numero 
total de preguntas, en tal caso se pasará a la pantalla final.

En la pantalla final, aprovechando el anterior condicional, saltará el "score" y una música u otra dependiendo de la puntuación, así como una frase distinta.
Por último, se ha añadido el botón volver a jugar, que reinicia el quiz a la primera pregunta
