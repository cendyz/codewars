Task:

Return the number (count) of vowels in the given string.

We will consider a, e, i, o, u as vowels for this Kata (but not y).

The input string will only consist of lower case letters and/or spaces.

Solution:

```ts
export class Kata {
  static getCount(str: string): number {
    const searchChars = ['a', 'e', 'i', 'o', 'u']
	return str.split('').filter(el => searchChars.includes(el)).length
  }
}
