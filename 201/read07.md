# Read07

## ¿Qué es la abstracción en programación y cómo se implementa utilizando objetos en JavaScript? Proporciona un ejemplo práctico

Es un metodo de simplificacion mediante el uso de objetos y clases.

Ejemplo

Personaje

- nombre
- fuerza
- defensa
- contructor()
- moverse
- ataque()

## ¿Cuáles son los cuatro pilares de la Programación Orientada a Objetos y cómo se aplican en JavaScript?

- Abstracción
- Encapsulamiento
- Herencia
- Polimorfismo

## ¿Cuál es la diferencia entre un objeto literal y una clase en JavaScript? ¿Cuándo deberías usar cada uno?

La diferencia es que una clase puede usarse como plantilla para crear diferentes objetos usando los atributos de un objeto literal.

## ¿Cómo implementarías la herencia en JavaScript utilizando clases? Proporciona un ejemplo que demuestre la relación padre-hijo entre dos clases

```

class Humano {
  constructor(nombre) {
    this.nombre = nombre;
  }

  nombreRetornado() {
    return `${this.nombre} `;
  }
}

class Gringo extends Humano {
  constructor(name, test) {
    super(name); // Llama al constructor de la clase padre
    this.test = test; // Propiedad específica de Dog
  }

  fetch() {
    return  `el gringo ${this.name}, tiene la test ${this.test}.`;
  }
}


const persona = new Gringo("Rui", "blanco");

console.log(persona.nombreRetornado()); 
console.log(persona.fetch());

```