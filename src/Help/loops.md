# Loops

A _loop_ is a programming tool that is used to repeat a set of instructions. _Iterate_ is a generic term that means “to repeat” in the context of _loops_. A _loop_ will continue to _iterate_ until a specified condition, commonly known as a _stopping condition_, is met.

## *for...in* loops

```javascript
let namesArray = ['Mary Gallagher', 'John Sanin', 'Anthony Clark', 'Margaret Farrell']

for (const nameIndex in namesArray) {
  // Note how nameIndex is assigned item's INDEX from array
  console.log(
    nameIndex,
    "--",
    "Person's name is", names[nameIndex]
  )
}
```

<p class="codeblock-caption cc-image">
  Console logs from <code>for...in</code> loop:
</p>

![](./../assets/images/1-js/for-1.png)

## *for...of* loops

The `for...of` conditional statement is very similar to `for...in`. In the `for...of` expression, the per item assignment simply is the item in the array, rather than the index Number.

With `for...of`, we do not need to use the index accessor statement.

```javascript
// Using `names` array assigned above
for (const name of names) {
  // Note how name is assigned actual item from array
  console.log("Person's name is", name)
}
```

<p class="codeblock-caption cc-image">
  Console logs from <code>for...of</code> loop:
</p>

![](./../assets/images/1-js/for-of-1.png)

## For Loops with Conditions

Now you can combine for loops and conditionals to create more dynamic results.

Let's log any ages less than 30.

```javascript
let ages = [22, 53, 21, 55]

for (const a in ages) {
  if (ages[a] < 30) {
    console.log(ages[a], "-- Young whipper snappers!")
  }
  else {
    console.log(ages[a], "-- Huh. What is old, really?")
  }
}
```

<p class="codeblock-caption cc-image">
  Console logs from conditional statements in the above for loop:
</p>

![](./../assets/images/1-js/for-2-cond.png)