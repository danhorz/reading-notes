# read 10

## ¿Cuáles son las diferentes formas de declarar una función en JavaScript? Explica las diferencias entre una declaración de función, una expresión de función y una función flecha.

- La declaracion de una funcion es algo que queremos que un objeto realice y la funcion flecha a diferencia de una funcion normal solo admite una linea de codigo.

## ¿Qué es una función callback y por qué son importantes en JavaScript? Proporciona un ejemplo práctico de su uso.

- Llama una funcion dentro de otra.

- const mensaje = function() {  
    console.log("Este mensaje se muestra después de 3 segundos");
}
 
setTimeout(mensaje, 3000);

## ¿Cómo afecta el hoisting a las declaraciones de funciones? ¿Existe alguna diferencia en cómo se manejan las funciones declaradas versus las expresiones de función?

Con solo expresiones no se puede llamar a una funcion. Y el hoisting afecta si llamamos mal una funcion  

## En el contexto de callbacks, ¿qué es el “callback hell” y cuáles son las estrategias modernas para evitarlo?

son muchas sobrecargas en la callback. La solucion mas recomendada es el  Async y Await.