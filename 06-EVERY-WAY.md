# Moving every way

`magik.exsultus` works by changing your velocity in one direction - up.

But you can change your velcity in any direction.

Here is the source code for `magik.exsultus`:

```javascript
function main(power: number | string = 50) {
	let jumppower = parseFloat((power as string))
	if (isNaN(jumppower)) {
		return magik.dixit('You need to pass in a number to exsultus!')
	}
	/**
	 * The range of jumppower is -100% to 100%. Values less than zero cause a
	 * downward velocity. Values above 0 cause an upward velocity
	 */
	jumppower = Math.min(jumppower, 100)
	jumppower = Math.max(jumppower, -100)
	const BukkitVelocityScaleFactor = 3.9 // Max valid velocity
	const jumpVelocity = jumppower / 100 * BukkitVelocityScaleFactor
	const yDeltaV = jumpVelocity
	const xDeltaV = 0.0
	const zDeltaV = 0.0
	const Vector = Java.type('org.bukkit.util.Vector')
	self.setVelocity(new Vector(xDeltaV, yDeltaV, zDeltaV))
}
```

See if you can figure out how to change it to move you in a different direction.
