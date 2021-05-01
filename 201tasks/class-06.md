# WHAT IS AN OBJECT?
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSZz1Xb2_BXZDFHECa_Z5zKiZCWR0cgpVe1KGxrUYRFi7zOWt7LJrCaFIkJtM70Y_yZC8I&usqp=CAU)
JavaScript is designed on a simple object-based paradigm. An object is a collection of properties, and a property is an association between a name (or key) and a value. A property's value can be a function, in which case the property is known as a method. In addition to objects that are predefined in the browser, you can define your own objects. This chapter describes how to use objects, properties, functions, and methods, and how to create your own objects.

**Objects overview**

Objects in JavaScript, just as in many other programming languages, can be compared to objects in real life. The concept of objects in JavaScript can be understood with real life, tangible objects.

In JavaScript, an object is a standalone entity, with properties and type. Compare it with a cup, for example. A cup is an object, with properties. A cup has a color, a design, weight, a material it is made of, etc. The same way, JavaScript objects can have properties, which define their characteristics.

**Objects and properties**

A JavaScript object has properties associated with it. A property of an object can be explained as a variable that is attached to the object. Object properties are basically the same as ordinary JavaScript variables, except for the attachment to objects. The properties of an object define the characteristics of the object. You access the properties of an object with a simple dot-notation:

![](https://fireship.io/courses/javascript/img/js-object-props.png)

## access an object and dot notation
![](https://miro.medium.com/max/1200/1*A-4sX6lswNKoDpuK3B90uQ.png)

**Syntax**
object.property
object['property']
## Updating Object Property

onst object1 = { property1: "Value 1" };
const object2 = { property2: "Value 2" };

const listOfObjects = [object1, object2];
const copyOfListOfObjects = [...listOfObjects];

function updateObjects(objects) {
  return objects.map((object) => {
    Object.keys(object).forEach((property) => {
      object[property] = "Updated value";
    });

    return object;
  });
}

const listOfUpdatedObjects = updateObjects(listOfObjects);

console.log(listOfObjects);
console.log(copyOfListOfObjects);
console.log(listOfUpdatedObjects);

![Updating Object Property
](https://i.ibb.co/8KbZ4mn/1.png)

## CREATING MANY OBJECTS:

**CONSTRUCTOR NOTATION**
Sometimes you will want several objects to represent similar things.
Object constructors can use a function as a template for creating objects.
First, create the template with the object's properties and methods.
![](https://miro.medium.com/max/3432/1*AlFcybVX3m9yXz01LcWa_A.png)

![](https://miro.medium.com/max/3916/1*2s2U-uXrRGFrkqYaFhBBUA.png)


