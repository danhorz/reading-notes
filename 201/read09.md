# read 9

## ¿Qué es un prototipo en JavaScript y cómo se relaciona con la herencia? Proporciona un ejemplo de cómo crear una cadena de prototipos

- El prototipo en si es un objeto y puede obtener caracteristicas propias  o de otros. Cuando se obtine una relacion con otros es llamdo herencia.
let animal = {
  name: "Animal",
  eat() {
    alert(`${this.name} come.`);
  }
};

let rabbit = {
  __proto__: animal,
  eat() {
    // ...rebota al estilo de conejo y llama al método padre (animal)
    this.__proto__.eat.call(this); // (*)
  }
};

let longEar = {
  __proto__: rabbit,
  eat() {
    // ...haz algo con orejas largas y llama al método padre (rabbit)
    this.__proto__.eat.call(this); // (**)
  }
};

longEar.eat();

## Cuando hablamos de la relación Modelo/Instancia en JavaScript, ¿qué diferencia existe entre una clase y una instancia de esa clase? ¿Cómo se crean las instancias?

Clase es un objeto con asignandole caracteristicas y una instancia declara este objeto con denominando cada caracteristica

## ¿Cómo funciona la herencia de propiedades y métodos en JavaScript? Explica el concepto de la cadena de prototipos con un ejemplo práctico

Por ejemplo tenemos un clase gato y una animal que posee las caracteristicas de caminar. Entonces gato heredara caminar a sus caracteristicas propias.

## ¿Cuáles son las mejores prácticas al implementar herencia en JavaScript? ¿Cuándo deberías usar herencia y cuándo podrías considerar otras alternativas?

- Llamar con super al padre
- Utilizar extents correctamente para añadir propiedades adicionales
