# Let's Describe Our Dog with Code!

Welcome to this tutorial! First off, this tutorial is meant for beginners in JavaScript, and will attempt to walk through core concepts with a build up to more complex programming ideas.

This first module - _Let's Describe Our Dog with Code_ will attempt to help you learn about:

- [What is an Object](#what-is-an-object)
- [What are Object Properties](#what-are-object-properties)
- [Objects and Properties in JavaScript](#objects-and-properties-in-javascript)
- [Key Value pairs](#key-value-pairs)
- [camelCasing](#camelcasing)
- Variables
- Strings
- Numbers
- Booleans

<!-- So let's start!

JavaScript is what's known as an **Object Oriented** programming langauge.

To put into  -->

## What is an Object?

In the kind of world we live in, we see _objects_ all around us. From the device you're using to read this tutorial, the chair you may be sitting in, to even you yourself!

Now we don't typically think of humans in the same way we think of computers and chairs, but we can describe all three (humans, computers, and chairs) as _objects_.

_Objects_ typically start with the _noun_ that names the _thing_ we are ultimately trying to describe.

For example, read the following and think about what comes to mind:

_I am something with four legs. You typically sit on me when you're tired of standing, or are sitting next to a table. I can be made out of many things, but am typically built out of wood and metal. Sometimes I have wheels, sometimes I have arm rests, and sometimes you can even spin around in circles when sitting on me. What am I?_

Hopefully a _chair_ came to mind!

___

## What are Object Properties?

Now what we just did was _describe_ what a _chair_ is. We said that a _chair_ has legs, could be made out of materials like wood and metal, could have arm rests, wheels, and could even allow whom ever is sitting in the _chair_ to spin!

Now in programming, what we just used to describe the _chair_ are called _properties_.

_Properties_ are things that belong to the idea of a _chair_, but can be unique to each _chair_.

For exmaple, some _chairs_ have three legs, are made out of plastics, have no wheels, and do not let whom ever is sitting them spin in circles.

So we can think of a _chair_ as an _Object_ which has _properties_ that describe it.

___

## Objects and Properties in JavaScript

In JavaScript, we use curly braces: `{}` to encapsulate (a fancy word which means to surround) _properties_ we use to describe an _Object_.

So following the _chair_ example, we might describe a _chair_ in JavaScript like so:

```javascript
{
    numberOfLegs: 4,
    madeOutOf: 'Wood and Metal'
    numberOfWheels: 4,
    spins: true
}
```

Now don't worry if the above doesn't make sense just yet, we'll go through each line of code:

Notice how the first and last lines are our curcly braces `{}`. See how they open up and encapsulate all of the _properties_ we use to describe our _chair_ earlier? This is how you define an _Object_ in JavaScript.

### Key Value Pairs

Now after the first curly brace `{` we see the line of code: `numberOfLegs: 4`.

_Properties_ of _Objects_ are described using **key value pairs** - This means that there is a _key_ (`numberOfLegs`) which is paired with a _value_ (`4`).

Typically, the _key_ is the word (sometimes words) we use to name a _property_ on our _Object_, and the corresponding _value_ is what actually describes our _Object_.

So in `numberOfLegs: 4` we are using the _key_ `numberOfLegs` to name the _value_ `4` which describes how many legs our _chair_ has.

### camelCasing

In JavaScript, it is convention (which means it is the agreed upon thing to do) to use what is called **camelCasing** when naming _properties_ that describe _Objects_ using multiple words.

So if we were to just use the word `legs` to describe the _number of legs_ our _chair_ has, we wouldn't need to use _camelCasing_ at all.

However, to make it easier for people to understand what our _property_ is describing on our _Object_ we use multiple words: `numberOfLegs`.

Notice how the first letter of each word after the first word, is capitalized - this is _camelCasing_.

There are a number of different casings, such as **PascalCasing** (which the first letter of each word is capatalized), but we don't need to know about those casings just yet.

For now, just understand that the first letter in each word after the first word, is capitalized when using _camelCasing_.

### Quick Summary

So far we learned that:

- `{}` represents our _Object_
- `numberOfLegs: 4` is a _property_ on our _Object_
- `numberOfLegs: 4` is also a **key value pair**, where `numberOfLegs` is our _key_,`4` is our _value_, and together they are a _pair_
- lastly, we learned that `numberOfLegs` uses the JavaScript naming convetion, called _camelCase_, to make the name of our _property_ more meaningful and easier to read