# Flexmix
> A Sass mixing that makes working with flexbox ease and quick!

### Install

You can get it on npm:
````
	npm install flexmix --save
````
or bower:
````
	bower install flexmix --save
````
### Setup
Just `@import` flexmix on your sass or scss file.

### Usage
#### So.. you wanna be a cool kid and use flexbox on your project? No problem!

flexmix is a easy to use, sass mixing (more like a shortcut) that helps you to write flexbox properties as quick as possible. check this out:

	.my-container{
	 @include flex-cont(row, nowrap, flex-start, center, center);
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


This is pretty straightforward and now you might know what I'm talking about. The only rule is the order of things. ***For now, flexmix only works if you follow this order of properties on the mixing:***

	flex-cont(flex-direction, flex-wrap, justify-content, align-items, align-content);

"Why?" you may ask. Well, at this moment I can't figure it out how to set us free from this, but if you, my dear fellow sass-hacker-master-coder-xtreme-developer know how to do it, just feel free to fork me =)

## ...but, you also may ask:
##### "Ok, I got it. But can I do this faster?"
##### "I have bills to pay! Can it be more quick?"
##### "My cat is having some trouble to poop in the right place, can you help me?"

My answer for you is: Yes! Sure! Probably not.

check this:

	my-second-container{			
	 @include fc(r, nw, fs, c, c);
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

Nice hum?

You can even use both ways and write the short version or the normal version of flexmix.

Now you can write flexbox properties really really fast, just follow the only rule and you're a good to go.

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


#### ***Have fun!***
