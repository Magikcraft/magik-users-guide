# Ingredients for Spells: Parameters

You can pass ingredients to your spells.

Magik users have their own secret language, and in that language ingredients for spells are called _parameters_.

To accept parameters in a spell, you need to write it in a special way, like this:

```javascript
const magik = magikcraft.io

function main() {
  magik.dixit('Hello World')
}
```
Write this spell and save it as `hw1`.

This spell has a _function_ in it, called "main". To get the ingredients in, we will add a parameter like this:

```javascript
const magik = magikcraft.io

function main(name) {
  magik.dixit('Hello World')
}
```

See how we put `name` in the brackets next to _main_?

That is how the ingredient will be passed in. Now we can use the ingredient in the spell, like this:

```javascript
const magik = magikcraft.io

function main(name) {
  magik.dixit('Hello ' + name)
}
```

Save the spell, then go to Minecraft and type: `/cast hw1`.

What do you see?

Your spell can take parameters, and you need to pass one in. To do that, go on to the next step.
