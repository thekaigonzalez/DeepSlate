# DeepSlate

DeepSlate allows you to traverse JavaScript Objects using a Python-like syntax.

## Example

```js

const DeepSlate = require("DeepSlate");

var obj = {
    firstNode: {
        secondNode: {
            string: "hello"
        }
    }
}

console.log(DeepSlate.traverse(obj, "firstNode.secondNode.string")) -> [Object "string"]



```

```js

const deepslate = require("./DeepSlate")

let o3 = {
    obj1: { obj2: 
        { obj3: 
            { obj4: 1+1 } 
        } 
    }
}
console.log("Object to traverse: ")
console.log(o3)

console.log(deepslate.traverse(o3, "obj1.obj2.obj3.obj4"));

2
```

