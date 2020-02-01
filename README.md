# Flexmix
> A Sass mixin that makes working with flexbox easy and quick!

### Update from the future 🚨
Really old project. Use with caution.

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
#### So.. do you wanna be a cool kid and use flexbox? No problem!

flexmix is a easy-to-use sass mixin(actually, more like a shortcut) that helps you to write flexbox properties as quickly as possible. check this out:

```
.my-container{
 @include flexmix(row, nowrap, flex-start, center, center);
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
```

*If you wanna know more about flexbox, see this [complete guide to flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) by Chris Coyier on css-tricks*

That was pretty easy! The only rule is the order of things. *For now, flexmix only works if you follow this order of properties on the mixin:*

`flex-direction` > `flex-wrap` > `justify-content` > `align-items` > `align-content`

## ...but, you may also ask:
##### "Ok, I got it. But can I do this quickly?"
##### "I have bills to pay! Can it be faster?"
##### "My cat is pooping in the wrong place, can you help me?"

My answer for you is: Yes! Sure! Probably not.

```
my-second-container{			
 @include flexmix(r, nw, fs, c, c);
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
```

just like that!

You can even shorten the mixin name to `@include flmx()` or `@include fm()`. In fact, you can mix everything. Whatever that works for you.

````
@include fm(row, nw, c, space-around, s);
````
*or*

````
@include flmx(row, rr, fs, baseline, center);
````
*or*

````
@include flexmix(rr, wr, c, s, c);
````


Now you can write flexbox properties really really fast. just follow the ***only rule*** and you're a good to go. Take a look on the shortcuts names bellow:

## Properties and shortcuts:

| flex-direction							| flex-wrap									| justify-content						|
| ------------- 							| -------------							|	-----------								|
| `row` *or* `r`  						| `wrap` *or* `w`						| `flex-start` *or* `fs`		|
| `row-reverse` *or* `rr`			| `nowrap` *or* `nw`				|	`flex-end` *or* `fe`			|
| `column` *or* `cl`					|	`wrap-reverse` *or* `wr`	|	`center` *or* `c`					|
| `column-reverse` *or* `clr`	|														|	`space-between` *or* `sb`	|
|															|														|	`space-around` *or* `sa`	|

| align-items									| align-content							|
| ------------- 							| -------------							|
| `flex-start` *or* `fs`  		| `flex-start` *or* `fs`		|
| `flex-end` *or* `fe`				|	`flex-end` *or* `fe`			|
| `center` *or* `c`						|	`center` *or* `c`					|
| `baseline` *or* `b`					|	`space-between` *or* `sb`	|
|	`stretch`	*or*  `s`					|	`space-around` *or* `sa`	|
|															|	`stretch`	*or*  `s`				|

**disclaimer:** For now, I don't have any plans to make flexmix work for flexbox items, because of the `flex:` shorthand that is already really easy to use.



## License

This project is licensed under the terms of the [MIT License](http://mit-license.org/).
