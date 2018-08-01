# sweep-and-prune

Incremental 2D sweep and prune collision detection for JavaScript.

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=Z2G8VHLDJ9N3L&lc=GB&item_name=Stefan%20Hedman&item_number=schteppe&currency_code=USD&bn=PP%2dDonationsBF%3aDonate%2dPayPal%2dgreen%2esvg%3aNonHosted)

## Installation

(TODO)

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
