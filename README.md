# Clases

En TypeScript, las clases son una parte fundamental de la programación orientada a objetos. Proporcionan una forma de definir estructuras y comportamientos reutilizables. Puedes crear una clase utilizando la palabra clave `class` seguida del nombre de la clase.

Aquí tienes un ejemplo básico de cómo crear una clase en TypeScript:

```typescript
class Person {
  name: string;
  age: number;

  constructor(name: string, age: number) {
    this.name = name;
    this.age = age;
  }

  sayHello() {
    console.log(`Hello, my name is ${this.name} and I'm ${this.age} years old.`);
  }
}
```

En este ejemplo, hemos creado una clase llamada `Person`. La clase tiene dos propiedades, `name` y `age`, y un constructor que acepta argumentos para inicializar esas propiedades. También tiene un método llamado `sayHello` que imprime un mensaje utilizando las propiedades de la instancia.

Para crear una instancia de la clase y utilizar sus propiedades y métodos, simplemente utilizamos el operador `new` seguido del nombre de la clase y los argumentos necesarios para el constructor:

```typescript
const person = new Person("John Doe", 25);
console.log(person.name); // John Doe
console.log(person.age); // 25
person.sayHello(); // Hello, my name is John Doe and I'm 25 years old.
```

En este ejemplo, hemos creado una instancia de la clase `Person` llamada `person` y hemos accedido a sus propiedades `name` y `age`. También hemos llamado al método `sayHello` para imprimir un mensaje.

Además de las propiedades y métodos, las clases en TypeScript también pueden tener modificadores de acceso como `public`, `private` y `protected`, que controlan la visibilidad y la accesibilidad de los miembros de la clase.

También es posible heredar de otras clases utilizando la palabra clave `extends`, lo que permite la creación de jerarquías de clases y la reutilización de código a través de la herencia.
