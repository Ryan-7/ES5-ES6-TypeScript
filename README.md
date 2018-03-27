# ES5-ES6-TypeScript

Wrapping my head around all of this syntactic sugar... 

// JavaScript before 'Class' keyword

function Person(name) {
  this.name = name;
  this.location = 'Madison';
}
Person.prototype.getInfo = function() {
  console.log(`My name is ${this.name} and I'm from ${this.location}`)
}
 
 
// ES6 Classes 
class Person {
  constructor(name) {
    this.name = name;
    this.location = 'Madison';
  }
  
  getInfo() {
    console.log(`My name is ${this.name} and I'm from ${this.location}`)
  }
}
 
 
// ES6 classes with proposed class properties 
class Person {
  location = 'Madison';
  constructor(name) {
    this.name = name;
  }
  getInfo = () => {
    console.log(`My name is ${this.name} and I'm from ${this.location}`)
  }
  
}
 
 
// TypeScript
class Person {
  location = 'Madison';
   constructor(name) {
    this.name = name;
  }
 
  getInfo() {
    console.log(`My name is ${this.name} and I'm from ${this.location}`)
  }
}
