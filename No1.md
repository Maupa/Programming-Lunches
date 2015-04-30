# Quadratic Equation
```js
Array.protype.qs = function(){
    var solutions = [];
    var a = this[0],
        b = this[1],
        c = this[2];
    for(var i = 0; i < 2; i ++)
        solutions.push(
                ( -b * Math.pow(-1, i) * Math.sqrt( Math.pow( b, 2 ) - 4 * a * c ))/( 2 * a )
            );
    return solutions;
}
```