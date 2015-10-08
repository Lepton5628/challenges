---
layout: post
title: "Challenge One"
date: "2015-9-26 20:28:00"
permalink: /2015/9/26/challenge-one
---
# Test Code

{% highlight javascript %}
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
{% endhighlight %}

# The Challenge

You must write a function `Random`.
It will have two parameter: `min` and `max`.

It will return a value between min and max such that:

{% highlight javascript %}
 min <= Random(min, max) < max
{% endhighlight %}

### Tools
Math.Random()  
returns a floating point between 1 & 0

The modulo (remainder operator): `%`

{% highlight javascript %}
5 % 2 = 1
5 % 3 = 2

remainder = a % b
{% endhighlight %}

 The modulo operator divides `a` by `b` and returns the REMAINDER.

 Good Luck!
