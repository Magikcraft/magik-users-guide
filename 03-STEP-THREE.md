# Passing in parameters

In the previous step you created a spell that can take a parameter (ingredient).

Now, you will learn how to pass a parameter into a spell.

In Minecraft, type `/cast hw1 There!`.

What do you see?

The word you typed after `hw1` is passed in as the parameter to your spell.

Parameters are separated by spaces, so you can't pass a sentence in as a single parameter, only a word.

You can make your spell take more than one parameter, like this:

```javascript
const magik = magikcraft.io

function main(firstname, lastname) {
  magik.dixit('Hello ' + firstname + ' ' + lastname)
}
```

Try that spell. When you cast it, pass in two names, like this: `/cast hw1 Jane Doe!`

You can make a spell that reads *all the parameters*, like this:

```javascript
const magik = magikcraft.io

function main(...name) {
  magik.dixit('Hello ' + name.join(' '))
}
```
Now you can give it as many names as you want!
