# Test Code

```javascript
var tests_number = 10000;

var global_min;
var global_max;

for(var i = 0;i < tests_number;i++){
	var r = Random(global_min, global_max);

	if(r < global_min || r > global_max){
		console.log('Tests failed!');

		// Don't wory about this, it's NodeJS. It exits the program.
		process.exit(1);
	}
}
```

# The Challenge

You must write a function ``Random''.
It will have two parameter: ``min'' and ``max''.

It will return a value between min and max such that:

 min <= Random(min, max) < max

### Tools
Math.Random()  
returns a floating point between 1 & 0

The modulo (remainder operator): `%`

```javascript
 5 % 2 = 1
 5 % 3 = 2

 a % b
```

 The modulo operator divides `a` by `b` and returns the REMAINDER.

 Good Luck!
