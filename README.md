# Flexmix
> A Sass mixing that makes working with flexbox ease and quick!

### Installation

You can get it on npm:
````
	npm install flexmix --save
````
or bower:
````
	bower install flexmix --save
````
### Setup
Just `@import` flexmix in your sass or scss file and you're good to go.

### Usage
#### So.. you wanna be a cool kid and use flexbox on your project? No problem!

flexmix is a easy to use sass mixing (actually, more like a shortcut) that helps you to write flexbox properties as quick as possible. check this out:

	.my-container{
	 @include flex-container(row, nowrap, flex-start, center, center);
	}

	// results in:
	.my-container{
	 display: flex;
	 flex-direction: row;
	 flex-wrap: nowrap;
	 justify-content: flex-start;
	 align-items: center;
	 align-content: center;
	}
	
*If you wanna know more about flexbox, check this [complete guide to flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) by Chris Coyier on css-tricks*

That was pretty straightforward. The only rule is the order of things. *For now, flexmix only works if you follow this order of properties on the mixing:*

`flex-direction` > `flex-wrap` > `justify-content` > `align-items` > `align-content`

"Why?" you may ask. Well, at this moment I can't figure it out how to set us free from this, but, if you my dear fellow sass-hacker-master-coder-extreme-developer know how to do it, just feel free to fork me =)

## ...but, you also may ask:
##### "Ok, I got it. But can I do this quickly?"
##### "I have bills to pay! Can it be more faster?"
##### "My cat is having some trouble to poop in the right place, can you help me?"

My answer for you is: Yes! Sure! Probably not.

check this:

	my-second-container{			
	 @include flex-container(r, nw, fs, c, c);
	}

	// results in:
	my-second-container{
	 display: flex;
	 flex-direction: row;
	 flex-wrap: nowrap;
	 justify-content: flex-start;
	 align-items: center;
	 align-content: center;
	}

just like that!

You can even shorten the mixing name to `@include fc()` and use both ways to write. In fact, you can mix it up everything.
````

	@include fc(row, nw, c, space-around, s);

````
*or*

````

	@include flex-container(cl, rr, fs, baseline, center);

````


Now you can write flexbox properties really really fast. just follow the ***only rule*** and you're a good to go. Take a look on the shortcuts names bellow and have fun!

## Properties shortcuts:

| flex-direction					| flex-wrap							| justify-content 			|
| ------------- 					| -------------					|	-----------						|
| `row` *or* `r`  						| `wrap` *or* `w`						| `flex-start` *or* `fs`		|
| `row-reverse` *or* `rr`			| `nowrap` *or* `nw`				|	`flex-end` *or* `fe`			|
| `column` *or* `cl`					|	`wrap-reverse` *or* `wr`	|	`center` *or* `c`					|
| `column-reverse` *or* `clr`	|												|	`space-between` *or* `sb`	|
|													|												|	`space-around` *or* `sa`	|

| align-items							| align-content					|
| ------------- 					| -------------					|
| `flex-start` *or* `fs`  		| `flex-start` *or* `fs`		|
| `flex-end` *or* `fe`				|	`flex-end` *or* `fe`			|
| `center` *or* `c`						|	`center` *or* `c`					|
| `baseline` *or* `b`					|	`space-between` *or* `sb`	|
|	`stretch`	*or*  `s`					|	`space-around` *or* `sa`	|
|													|	`stretch`	*or*  `s`				|


**disclaimer:** For now, I don't have plans to make flexmix work for flexbox items because of the `flex:` shorthand that is already fast.

## License

This project is licensed under the terms of the [MIT License](http://mit-license.org/).
