# sweep-and-prune

## Documentation

### Constructor

```js
var sap = new SweepAndPrune();
```

### .addObject

```js
var data = { foo: "bar" };
var x0 = 0;
var y0 = 1;
var x1 = 2;
var y1 = 3;
var box = sap.addObject(x0,y0,x1,y1,data);
```

### .updateObject

```js
var x0 = 0;
var y0 = 1;
var x1 = 2;
var y1 = 3;
sap.updateObject(box,x0,y0,x1,y1);
```

### .removeObject

```js
sap.removeObject(box);
```

### .onadd

```js
sap.onadd = function(boxA, boxB){
  // Do something with boxA.userData or boxB.userData
};
```

### .onremove

```js
sap.onremove = function(boxA, boxB){
  // Do something with boxA.userData or boxB.userData
};
```
