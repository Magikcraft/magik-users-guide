# Manifesting Things Magikally

Now you will learn how to magically manifest items.

To do this, you will _require_ some more magik.

Make a new spell, and give it a cool name like `abracadabra`. Put this in it:

```javascript
const magik = magikcraft.io

const inventory = require('inventory')
const items = require('items')

function main() {

}
```

*const* is a special magical word for things that don't change. It is short for _constant_.

The magical word *require* brings in more magic that you can use.

Now you have magic for items and for the Minecraft inventory. The next thing you want to do in your spell is to get _your_ inventory. You do it like this:

```javascript
const magik = magikcraft.io

const inventory = require('inventory')
const items = require('items')

function main() {
  const myInventory = inventory(self)
}
```

*self* is a special magik term that means your Minecraft player in your spells.

Now that you have your inventory, you can add things to it, like this:

```javascript
const magik = magikcraft.io

const inventory = require('inventory')
const items = require('items')

function main() {
  const myInventory = inventory(self)
  myInventory.add( items.cookie(1) )
    .add( items.bakedPotato(1) )
}
```

Try that!

To get an idea of the kinds of things you can add to your inventory, [see this list](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/Material.html).

Not everything on there will work, but that is part of the fun of learning magik - and why it is so mysterious to those who have not studied and learned its ways...

[Go on](./05-LEAPING)!
