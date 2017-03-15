# arrTree
A library that allows you to create an object tree from a string and work with it.

### How to use? ###

Create object
```javascript
var myObj = {};
```

And add new values.
```javascript
//Create object
var myObj = {};

//And add new values.
ArrTree.set(myObj, 'myKey', 'myVal');
ArrTree.set(myObj, 'myKey.keyTree', 'treeVal');

//Get value
ArrTree.get(myObj, 'myKey.keyTree', undefined);

//Has key
ArrTree.has(myObj, 'myKey.keyTree');

//Remove key and val
ArrTree.remove(myObj, 'myKey.keyTree');
```

#### Available methods ####

* __set(obj, key, val)__: Set object value.
* __get(obj, key, defaultVal)__: Get the value of the key. If the key is not found, it returns DefaultVal.
* __has(obk, key)__: Check if a key is detected. Return bool.
* __remove(obj, key)__: Removes a key from the object. Return bool.