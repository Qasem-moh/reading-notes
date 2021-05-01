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

---

# Document Object Model in JavaScript

**What is Document Object Model (DOM)**

The Document Object Model (DOM) is an application programming interface (API) for manipulating HTML and XML documents.

The DOM represents a document as a tree of nodes. It provides API that allows you to add, remove, and modify parts of the document effectively.

Note that the DOM is cross-platform and language-independent ways of manipulating HTML and XML documents.

A document as a hierarchy of nodes
The DOM represents an HTML or XML document as a hierarchy of nodes. Consider the following HTML document:
![](https://i.ibb.co/MhhmMCX/11.png)

![](https://www.javascripttutorial.net/wp-content/uploads/2020/01/JavaScript-DOM.png)

n this DOM tree, the document is the root node. The root node has one child which is the <html'> element. The <html'> element is called the document element.

Each document can have only one document element. In an HTML document, the document element is the <html'> element. Each markup can be represented by a node in the tree.

**Node Types**

Each node in the DOM tree is identified by a node type. JavaScript uses integer numbers to determine the node types.

The following table illustrates the node type constants:
![](https://i.ibb.co/R6FwBgK/111.png)

To get the type of a node, you use the nodeType property:
**node.nodeType**

_The nodeName and nodeValue properties_
_A node has two important properties: nodeName and nodeValue that provide specific information about the node._

The values of these properites depends on the node type. For example, if the node type is the element node, the nodeName is always the same as element’s tag name and nodeValue is always null.

For this reason, it’s better to test node type before using these properties:

**if (node.nodeType == Node.ELEMENT_NODE) {**
    **let name = node.nodeName; // tag name like <p'>**
**}**


**Node and Element**

Sometime, it’s easy to confuse between the Node and the Element.

A node is a generic name of any object in the DOM tree. It can be any built-in DOM element such as the document. Or it can be any HTML tag specified in the HTML document like <div'> or <p'>. 

An element is a node with a specific node type Node.ELEMENT_NODE, which is equal to 1.

In other words, the node is generic type of the element. The element is a specific type of the node with the node type Node.ELEMENT_NODE.

The following picture illustrates the relationship between the Node and Element types:

![](https://www.javascripttutorial.net/wp-content/uploads/2020/01/Document-Object-Model-in-JavaScript.png)

Note that the getElementById() and querySelector() returns an object with the Element type while getElementsByTagName() or querySelectorAll() returns NodeList which is a collection of nodes. 

Node Relationships
Any node has relationships to other nodes in the DOM tree. The relationships are the same as the one described in a traditional family tree.

For example, <body'> is a child node of the <html'> node, and <html'> is the parent of the <body'> node.

The <body'> node is the sibling of the <head'> node because they share the same immediate parent, which is the <html'> element.