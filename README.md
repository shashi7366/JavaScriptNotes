# JavaScriptNotes

## data types in javascript

Wrapper Objects
Objects are always truthy in if

Let a=123
A.toString(base)

0x-hex
0b-binary
0o-octal

Math.floor();
Math.ceil()
Math.round()

1e6
1e-6

123..tofixed(1)
123..toString()

isNaN(a);
isFinite(a)

Number.isNaN();
Number.isFinite();

Numeric conversion using a plus + or Number() is strict. If a value is not exactly a number, it fails:

alert( +"100px" ); // NaN


alert( parseInt('100px') ); // 100
alert( parseFloat('12.5em') ); // 12.5

alert( parseInt('12.3') ); // 12, only the integer part is returned
alert( parseFloat('12.3.4') ); // 12.3, the second point stops the reading

alert( parseInt('a123') ); // NaN, the first symbol stops the process

alert( parseInt('0xff', 16) ); // 255
alert( parseInt('ff', 16) ); // 255, without 0x also works

alert( parseInt('2n9c', 36) ); // 123456
