# How to Train a Dog with JavaScript

**Disclaimer** I used this wonderful tutorial as inspiration: http://jsforcats.com/

This is spot:

```javascript
'Spot'
```

He's not much right now...not even a dog really, but he has a name and while we can imagine him, and the things dogs usually do, we can make him come alive with **JavaScript**!

So as you saw above, right now `Spot` is just a name. A name in which is contained in single quotes: `'Spot'`
In **JavaScript**, there is an idea of `strings` for what you and I might call words.

When you want to say something in **JavaScript**, you wrap your words or sentences in either single `''` or double `''` quotes.

Usually it's preferred you contain your words and sentences within single quotes `''`, but sometimes we have words that have quotes in them, for example:
- `Spot's favorite color is red!`
- `Spot doesn't really know many tricks yet`
- `Spot said his favorite quote was "every dog has his day"`

So usually, if you know what you want to say doesn't include any quotes, you should wrap your words and sentences in `''` single quotes, but if you need to use a word or sentence which contains quotes, use them like this:

- `"I'm a sentence that contains a single quotes, so I'm wrapped in double quotes!"`
- `'There are no single quotes in me, so wrap me in single quotes!'`
- `There are double quotes in this sentence, "every dog has his day", but no single quotes, so wrap me in single quotes!`

So as you can see, there's nothing particularly fancy about `strings`, besides when you should wrap them in single or double quotes.

Now we know that `Spot` is really only a `string` right now, not really a dog, so what can we do about that?

Well we can give him so more characteristics to describe what he's like:

```javascript
'Spot'
'brown fur'
'blue eyes'
'red collar'
```

So what if we wanted to say how old `Spot` is? Of course we could say he's `'four years old'`, but what if we want to say how old he'd be in another four years? We don't typically do math with words, we use numbers!

Well luckily, JavaScript also supports numbers:

```javascript
2
42
720
3452
```

So instead of saying, '`Spot is four years old'` we can add it to our list of characteristic describing him like this:

```javascript
'Spot'
'brown fur'
'blue eyes'
'red collar'
4
```

But now is just listing `4` like we have very clear about what it represents for `Spot`? I'd argue most people wouldn't have a clue what a random `4` means, so let's give these `strings` and `integers` (`integers` are what we call **numbers** in **JavaScript**) some useful descriptors:

```javascript
let name = 'Spot'
let furColor = 'brown'
let eyeColor = 'blue'
let collarColor = 'red'
let yearsOld = 4
```