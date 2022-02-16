# TECHICAL PAPER - OBJECTS

## Introduction to Objects

* There are only seven fundamental data types in JavaScript, and six of those are the primitive data types: string, number, boolean, null, undefined, and symbol. With the seventh type, objects, we open our code to more complex possibilities.
* An object is a collection of properties, and a property is an association between a name (or key) and a value.

![This is an image](https://content.codecademy.com/courses/learn-javascript-objects/javascript_illo.svg )


## Creating Object Literals

Objects can be assigned to variables just like any JavaScript type. We use curly braces, {}, to designate an object literal:

 ```let spaceship = {}; // spaceship is an empty object```

We fill an object with unordered data. This data is organized into key-value pairs. A key is like a variable name that points to a location in memory that holds a value.

![](https://content.codecademy.com/courses/learn-javascript-objects/key%20value.svg)

```
// An object literal with two key-value pairs
let spaceship = {
  'Fuel Type': 'diesel',
  color: 'silver'
};        
```
