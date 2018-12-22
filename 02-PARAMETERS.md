# Ingredients for Spells: Parameters

You can pass ingredients to your spells.

A spell is like a recipe, and you can write spells that take different ingredients whenever you cast them.

Magik users have their own secret language, and in that language ingredients for spells are called _parameters_. Spells are called programs.

To accept parameters in a spell, you need to write it in a special way, like this:

```javascript
const magik = magikcraft.io

function main() {
  magik.dixit('Hello World')
}
```
Write this spell and save it as `hw1`.

This spell has a _function_ in it, called "main". This is a special function in a Magikcraft spell. You can have many functions in a spell, but the one named `main` is the one that is called when you cast the spell in Minecraft.

To get the ingredients into the spell, we will add a parameter like this:

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

You might see something like: `Hello undefined`.

When you cast a spell in Minecraft that takes ingredients, you need to give it specific ingredients to use. When you pass the ingredients in as you cast the spell, they are called _arguments_.

Your spell can take parameters, and now you need to pass one in as an argument. To find out how to do that, go on to [the next step](./03-PARAMETERS-2).
