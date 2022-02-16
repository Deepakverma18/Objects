# TECHICAL PAPER - OBJECTS

## Introduction to Objects

* There are only seven fundamental data types in JavaScript, and six of those are the primitive data types: string, number, boolean, null, undefined, and symbol. With the seventh type, objects, we open our code to more complex possibilities.
* An object is a collection of properties, and a property is an association between a name (or key) and a value.

![This is an image](https://content.codecademy.com/courses/learn-javascript-objects/javascript_illo.svg )

## Creating Object Literals

Objects can be assigned to variables just like any JavaScript type. We use curly braces, {}, to designate an object literal:

 ```
 let spaceship = {}; // spaceship is an empty object
 ```

We fill an object with unordered data. This data is organized into key-value pairs. A key is like a variable name that points to a location in memory that holds a value.

![This is Image](https://content.codecademy.com/courses/learn-javascript-objects/key%20value.svg)

```
// An object literal with two key-value pairs
let spaceship = {
  'Fuel Type': 'diesel',
  color: 'silver'
};        
```

## Accessing Properties

There are two ways we can access an object’s property.

* Dot notation(.)
* Bracket notation [].

Let us see first notation i.e. Dot notation-

```
'hello'.length; // Returns 5
```

With property dot notation, we write the object’s name, followed by the dot operator and then the property name (key):

```
let spaceship = {
  homePlanet: 'Earth',
  color: 'silver'
};
spaceship.homePlanet; // Returns 'Earth',
spaceship.color; // Returns 'silver',
```

Let us see second notation i.e Bracket notation.

We've used bracket notation when indexing an array:

```
['A', 'B', 'C'][0]; // Returns 'A'
```
To use bracket notation to access an object’s property, we pass in the property name (key) as a string.

```
let spaceship = {
  'Fuel Type': 'Turbo Fuel',
  'Active Duty': true,
  homePlanet: 'Earth',
  numCrew: 5
};
spaceship['Active Duty'];   // Returns true
spaceship['Fuel Type'];   // Returns  'Turbo Fuel'
spaceship['numCrew'];   // Returns 5
spaceship['!!!!!!!!!!!!!!!'];   // Returns undefined
```

With bracket notation you can also use a variable inside the brackets to select the keys of an object. This can be especially helpful when working with functions:

```
let returnAnyProp = (objectName, propName) => objectName[propName];
 
returnAnyProp(spaceship, 'homePlanet'); // Returns 'Earth'
```











