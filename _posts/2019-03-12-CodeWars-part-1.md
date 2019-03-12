---

---

[CodeWars](https://www.codewars.com) is a website where you are given challenges and must write code that satisfies requirements.  

These are some challenges and my thinking behind my answer.

### Challenge: Find the smallest integer in the array
This is a sorting problem.  My initial reaction is to sort the array from largest to smallest and return the last entry.  I will have to look at some array methods to know what to do.

I searched on [W3Schools](https://www.w3schools.com/js/js_array_sort.asp) for the various array methods.  

There are several methods of finding the minimum or maximum values of an array.  One is to compare numbers and use the ```sort()``` method.  For numbers, this requires another function to see if the numbers create a negative, 0, or positive number.  This is because of the hierarchy in numbers.  20 > 100 in computer talk.  :)  

The method I used was to use the Math method to identify the minimum value.  Here's the code I copied: ```Math.min.apply(null, args)```.  I don't fully understand the apply or the need for ```null```.  I will look that up.

The ```apply()``` method adds arguments found in an array to an object.  We didn't have an object, so ```null``` was needed.

Here is the best practice code: ```Math.min(...args)```.
The spread, ```...``` gives a comma separated list which the ```min()``` can use.  

### Challenge: Write a program that finds the summation of every number from 1 to number

My idea is to create a variable to keep track of the summation.  Then, run a for-loop until the index variable matches the number given.

Hooray!  That happened to be best practice.  However, I saw some answers using an arrow function and the Fibonacci sequence to solve the problem.  

Here's that code: ```const summation = n => n * (n + 1) / 2;```.  

I didn't see that coming.  I will need to spend time looking at Arrow functions.


Keep Evolving!
