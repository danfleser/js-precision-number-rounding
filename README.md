# js-precision-number-rounding
Js precision number rounding toFixed replacement


```javascript
function truncateNumber(num, dec = 2) {
  const calcDec = Math.pow(10, dec);
  return Math.trunc(num * calcDec) / calcDec;
}

// this is not ok
4.199.toFixed(2);// => 4.20
// this is what we want
truncateNumber(4.199, 2);// = 4.19
```
