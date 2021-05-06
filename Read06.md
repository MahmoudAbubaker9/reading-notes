# Loops and iteration

**Loops offer a quick and easy way to do something repeatedly**

>Example : for (let step = 0; step < 5; step++) {
  // Runs 5 times, with values of step 0 through 4.
  console.log('Walking east one step');
}


**for statement**

A for loop repeats until a specified condition evaluates to false.

>for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement

**do...while statement**

The do...while statement repeats until a specified condition evaluates to false.

>In the following example, the do loop iterates at least once and reiterates until i is no longer less than 5.

>let i = 0;
 do {
  i += 1;
  console.log(i);
} while (i < 5);

**while statement**

If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

>Example: 

>let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}


**There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times**

The statements for loops provided in JavaScript are:

1-labeled statement

2-break statement

3-continue statement

4-for in statement

5-for of statement

[Ref](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)
