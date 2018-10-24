# NodeJS-readFile-vs-Stream
This example is very usefull for the difference between readFile() and createReadStream() in NodeJS

Step1: Execute create-csv-file.js and it will create 4 csv files with data and different size 

Step2: Execture the read.js file then you can see in the console file reading times from both approach readFile() and createReadStream()


Here we can see the ES6&ES7 feature like Async/Await usage.

The word “async” before a function means one simple thing: a function always returns a promise. If the code has return <non-promise> in it, then JavaScript automatically wraps it into a resolved promise with that value.
For instance, the code above returns a resolved promise with the result of 1, let’s test it:
async function f() {
  return 1;
}

f().then(alert); // 1

We could explicitly return a promise, that would be the same:
async function f() {
  return Promise.resolve(1);
}

f().then(alert); // 1
So, async ensures that the function returns a promise, and wraps non-promises in it. Simple enough, right? But not only that. There’s another keyword, await, that works only inside async functions, and it’s pretty cool.
