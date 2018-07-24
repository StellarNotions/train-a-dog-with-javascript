# Let's Describe Our Dog with Code!

Welcome to this tutorial! First off, this tutorial is meant for beginners in JavaScript, and will attempt to walk through core concepts with a build up to more complex programming ideas.

This first module - _Let's Describe Our Dog with Code_ will attempt to help you learn about:

- [Let's Describe Our Dog with Code!](#lets-describe-our-dog-with-code)
    - [What is Syntax](#what-is-syntax)
    - [What is an Object](#what-is-an-object)
        - [What are Object Properties](#what-are-object-properties)
        - [Objects and Properties in JavaScript](#objects-and-properties-in-javascript)
        - [Key Value Pairs](#key-value-pairs)
        - [camelCasing](#camelcasing)
        - [Quick Review](#quick-review)
    - [What are Comments](#what-are-comments)
    - [Numbers](#numbers)
    - [Strings](#strings)
    - [Booleans](#booleans)
    - [Let's Review](#lets-review)
    - [Time to Describe Our Dog](#time-to-describe-our-dog)
        - [What's null](#whats-null)

## What is Syntax

Like sentences have structure we call _grammar_, code has structure we call _syntax_.

_Syntax_ describes how we write our code, and can differ between each programming language.

---

## What is an Object

In the kind of world we live in, we see _objects_ all around us. From the device you're using to read this tutorial, the chair you may be sitting in, to even you yourself!

Now we don't typically think of humans in the same way we think of computers and chairs, but we can describe all three (humans, computers, and chairs) as _objects_.

_Objects_ typically start with the _noun_ that names the _thing_ we are ultimately trying to describe.

For example, read the following and think about what comes to mind:

_I am something with four legs. You typically sit on me when you're tired of standing, or are sitting next to a table. I can be made out of many things, but am typically built out of wood and metal. Sometimes I have wheels, sometimes I have arm rests, and sometimes you can even spin around in circles when sitting on me. What am I?_

Hopefully a _chair_ came to mind!

### What are Object Properties

Now what we just did was _describe_ what a _chair_ is. We said that a _chair_ has legs, could be made out of materials like wood and metal, could have arm rests, wheels, and could even allow whom ever is sitting in the _chair_ to spin!

Now in programming, what we just used to describe the _chair_ are called _properties_.

_Properties_ are things that belong to the idea of a _chair_, but can be unique to each _chair_.

For example, some _chairs_ have three legs, are made out of plastics, have no wheels, and do not let whom ever is sitting them spin in circles.

So we can think of a _chair_ as an _Object_ which has _properties_ that describe it.

### Objects and Properties in JavaScript

In JavaScript, we use curly braces: `{}` to encapsulate (a fancy word which means to surround) _properties_ we use to describe an _Object_.

So following the _chair_ example, we might describe a _chair_ in JavaScript like so:

```javascript
{
    numberOfLegs: 4,
    madeOutOf: 'Wood and Metal',
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

Notice how we type a `:` between our _key_ and our _value_, this is the [**syntax**](#what-is-syntax) JavaScript uses to tell the difference between what our _key_ is, and what _value_ it holds.

### camelCasing

In JavaScript, it is convention (which means it is the agreed upon thing to do) to use what is called **camelCasing** when naming _properties_ that describe _Objects_ using multiple words.

So if we were to just use the word `legs` to describe the _number of legs_ our _chair_ has, we wouldn't need to use _camelCasing_ at all.

However, to make it easier for people to understand what our _property_ is describing on our _Object_ we use multiple words: `numberOfLegs`.

Notice how the first letter of each word after the first word, is capitalized - this is _camelCasing_.

There are a number of different casings, such as **PascalCasing** (which the first letter of each word is capatalized), but we don't need to know about those casings just yet.

For now, just understand that the first letter in each word after the first word, is capitalized when using _camelCasing_.

### Quick Review

So far we learned that:

- `{}` represents our _Object_
- `numberOfLegs: 4` is a _property_ on our _Object_
- `numberOfLegs: 4` is also a **key value pair**, where `numberOfLegs` is our _key_,`4` is our _value_, and together they are a _pair_ separated by a `:`
- lastly, we learned that `numberOfLegs` uses the JavaScript naming convention, called _camelCase_, to make the name of our _property_ more meaningful and easier to read

---

## What are Comments

In JavaScript, we can write helpful messages to ourselves, and other developers using two forward slashes ``//`` to write **comments**

```javascript
// Comments will NOT be ran as code, but will instead be ignore by JavaScript.
```

You write multi-line comments using `/**/` like such:

```javascript
/*
   Here is a
   really long
   multi-line
   comment!
*/
```

---

## Numbers

In JavaScript, we express numeric values simply by just typing the numbers.

For example:

```javascript
42
3.14
524934 // The circumfrence of the Death Star in feet!
```

Are all **numbers** in JavaScript.

So regarding our _chair object_:

```javascript
{
    numberOfLegs: 4,
    madeOutOf: 'Wood and Metal',
    numberOfWheels: 4,
    spins: true
}
```

Our _keys_ `numberOfLegs` and `numberOfWheels` both hold the _value_ `4` which is a **number**.

We can do any form of arithmetic with **numbers** in JavaScript, such as:

```javascript
42 + 42   // Addition
450 - 30  // Subtraction
4 * 4     // Multiplication
100/25  // Division
2**8    // Exponents
```

Whenever we perform math operations using **numbers**, JavaScript will also give us back a **number** as a result.

This allows us to chain math operations like so:

```javascript
(42 + 450) - 30 + 4 * 4 + 100/25 + 2**8 // Which would equal 738
```

In JavaScript the **numbers** used in the math problems are known as _operands_ while the math operation being performed are known as _operators_.

```javascript
//  Operand   Operator   Operand
    3          +          2
```

Another _operator_ used in JavaScript is the _modulus_ operator, which is a fancy word for saying _what is the remainder of one operand divided by another operand_.

For example `15 % 2` means: _what is the remainder of 15 divided by 2_

```javascript
//  Operand   Modulus Operator   Operand
    15        %                  2           // Equals 1
```

## Strings

The next line in our _chair object_ is: `madeOutOf: 'Wood and Metal'`

Where `madeOutOf` is our _key_, and `'Wood and Metal'` is our value.

Now you may be wondering why _Wood and Metal_ is _encapsulated_ within single quotes (`''`)

This is what's known as a **string** in JavaScript.

You can think of **strings** as just words, and sentences.

```javascript
'This is a string!'
```

Typically we _encapsulate_ **strings** in JavaScript using single quotes: `''`, but it is also valid to use double quotes `""`

Using double quotes becomes necessary when we use words that already contain single quotes.

For example: `"it's"`

So when using words that already contain single quotes in JavaScript, we have two options:

1. We can _encapsulate_ the **string** in double quotes: `"it's"`
2. Or we can _escape_ the single quote like so: `'it\'s'`

The first option is what's most typically used, but there are cases where it's easier to _escape_ the single quote character

For instance, when you're quoting someone:

```javascript
'"No one in the brief history of computing has ever written a piece of perfect software. It\'s unlikely that you\'ll be the first." ~ Andy Hunt'
```

## Booleans

We've already gone over the _chair object property_ `numberOfWheels`, so the only _property_ remaining is `spins`

```javascript
{
    numberOfLegs: 4,
    madeOutOf: 'Wood and Metal',
    numberOfWheels: 4,
    spins: true
}
```

Now maybe your first thought is why we didn't _encapsulate_ the _value_ of the _object property_ `spins` in single or double quotes. It is a word right?

Well `true` and `false` are actually values in JavaScript that are called **Booleans**

They simply describe whether something is _true_ or _false_.

In our _chair object_ we use a **Boolean** to describe whether or not our _chair_ spins.

So one can assume that because the `spins` _property_ of our _chair_ is `true`, one could spin around in our chair until their heart's content.

## Let's Review

- **Syntax** is like code grammer. It's the sublte rules that dictate how we must write our code in order for JavaScript to understand what we're trying to do
- **Objects** are like objects in real life. They are _things_ in which we can _describe_
- **Object Properties** consists of **key value pairs** where the **key** is what we are describing about our **Object** and the **value** is how we are describing it
- **camelCasing** is a method used to name things in JavaScript
- **// comments** are helpful notes we can leave for ourselves, and other developers within our code
- **Numbers** are the same as in math, and are just typed by themselves (without single or double quotes encapsulating them)
- **Strings** are sentences or words in JavaScript, they can be encapsulated in single (`''`) or double (`""`) quotes
- **Booleans** are either `true` or `false` and they represent values that are either true or false, they should **NOT** be encapsulate within single or double quotes

## Time to Describe Our Dog

So now it's time to take everything we've learned so far, and put it all together to describe our dog!

I encourage you to be creative, and try to come up with a dog that's different than mine, as the end goal of these tutorials is to actually put a _real_ version of your dog out there on the internet for everyone to appreciate!

So let's start!

In terms of JavaScript, we know that our dog is a _thing_, because it has _properties_ we can describe, so let's start with an _object_:

```javascript
{
    // This will soon describe our super awesome dog
}
```

So let's start thinking about ways we can describe our dog:

- Name of our dog
- Gender of our dog
- What breed our dog is
- Age of our dog
- Fur color
- Eye color
- Whether he/she wears a collar
- If so, the color of his/her collar
- Our dog's favorite treat

I think with these _properties_ defined, we can get a pretty good idea of what our dog looks like, so let's turn the above list into code:

```javascript
{
    name: 'Arabella',
    gender: 'Female',
    breed: 'German Shepard',
    age: 4,
    furColor: 'Chocolate Brown',
    eyeColor: 'Nebula Blue',
    wearsACollar: true,
    colorOfCollar: 'Crimson',
    favoriteTreat: 'Peanut Butter'
}
```

Now if your dog doesn't wear a collar, you could represent that by doing the following:

```javascript
{
    name: 'Arabella',
    gender: 'Female',
    breed: 'German Shepard',
    age: 4,
    furColor: 'Chocolate Brown',
    eyeColor: 'Nebula Blue',
    wearsACollar: false,
    colorOfCollar: null,
    favoriteTreat: 'Peanut Butter'
}
```

### What's null

`null` is another value in JavaScript that actually represents the absence of a value, a little confusing, right?

Well JavaScript has to have a _value_ in a _key value pair_ or else it wouldn't be a pair.

So `null` is what you use when you don't have a _value_ to give a _key_, and because `null` is a value that represents no value, JavaScript doesn't have a problem with using it in a _key value pair_

So if your dog doesn't wear a collar (`wearsACollar: false`), how can your dog's collar have a color? Exactly! It can't!

But we can't leave the value empty, because JavaScript will give what's called a **syntax error** - Which means, we tried to write some code that wasn't _grammatically_ correct in JavaScript.

So if your dog doesn't wear a collar, we must represent the _property_ `colorOfCollar` as `null`, because there is no color for a collar that doesn't exist!