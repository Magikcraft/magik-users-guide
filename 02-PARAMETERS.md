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

You should see something like: `Hello undefined`.

Your spell can take parameters, and now you need to pass one in. To find out how to do that, go on to [the next step](./03-PARAMETERS-2).

## Common Problems

There are two common mistakes here:

1. Not putting the space in `'Hello '`. If you miss out the space after `Hello`, you will see `Helloundefined`. Spaces inside quotes - `'` or `"` - are interpreted literally. If you put two spaces in there, you will see two spaces in the message in Minecraft. If you put no spaces in there, you will see no space in Minecraft.

2. Not closing the braces - `{ }`. Every time you use an open bracket - `(` - or an open curly brace - `{` - you must close it. If you miss out the final closing brace - `}`, the spell will not work.

## Notes for Parents

If your child is working through this, coach them to look carefully at the instructions and following them precisely. If the spell is not working, go through each line, each character to verify that it is exactly as printed here. Think of a computer program like a telephone number or an email address. One wrong digit, one mis-spelled letter, and you don't get what you expect!

## Notes for Programmer Parents

The `main()` function is a convention that we use in Magikcraft to pass in arguments from the user console in Minecraft. The `main()` function in a Magikcraft spell, if present, is automatically invoked. Code in a spell outside a function is also automatically executed, but cannot receive input parameters.
