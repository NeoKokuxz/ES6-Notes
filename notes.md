# Notes
Link: https://www.learningcrux.com/course/the-complete-react-js-redux-course-build-modern-web-apps

## Let - Var - Const 
- Let 
  - can reassign value
  - doesn't leak outside of block scope like {}
- Var 
  - can reassign value 
  - can leak outside of scope, only temporary inside function scope
- Const
  - can't reassign value
  - doesn't leak outside of block scope {}
  - Exception : const object's property can be changed but no the object itself
  
## Arrow Function
```javascript
const integers = [1, 2, 3];
const updatedIntegers = integers.map( () => "neooo"); // ['neooo','neoooo','neoooo']
```

## Protoype Methods (ES5)
```javascript
function Person(name, age){
  this.name = name;
  this.age = age;
}

Person.prototype.speak = function(){
 console.log("My name is ${this.name} and my age is ${this.age}") //This will whatever the name and age belong to this method
}

const Neo = new Person("Neo", 20);

Neo.speak(); // My name is Neo and my age is 20
```

