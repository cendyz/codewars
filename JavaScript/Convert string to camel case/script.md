Task:

Complete the method/function so that it converts dash/underscore delimited words into camel casing. The first word within the output should be capitalized only if the original word was capitalized (known as Upper Camel Case, also often referred to as Pascal case). The next words should be always capitalized.
Examples

```js
"the-stealth-warrior" gets converted to "theStealthWarrior"

"The_Stealth_Warrior" gets converted to "TheStealthWarrior"

"The_Stealth-Warrior" gets converted to "TheStealthWarrior"
```

Solution:

```js
const toCamelCase = str => {
	return str
		.split(/[-_]/)
		.map((w, i) => (i === 0 ? w : w[0].toUpperCase() + w.slice(1)))
		.join('')
}
```
