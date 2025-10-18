# swe-sr-1-1

Welcome to your first short response assignment! If the code that you write is what gets your foot in the door for a job interview, how you communicate is what will get you the job. So, treat these assignments seriously! Write your responses as if you were planning on publishing them in a blog for the world to see (and, if you're confident, actually publish them!).

## Setup

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/how-tos/working-with-assignments#how-to-work-on-assignments).

Here are some useful commands to remember.

```sh
npm i                   # install dependencies
git checkout -b draft   # switch to the draft branch before starting

git add -A              # add a changed file to the staging area
git commit -m 'message' # create a commit with the changes
git push                # push the new commit to the remote repo
```

## Prompt

Imagine you are teaching a brand new programmer a brief lesson about functions and function calls. Your lesson should have the following components:

* A technical definition ("According to MDN, a function is...").
* An explanation of the concept with an analogy ("You can think of a function a ...")
* An example of the syntax for an arrow function using a JavaScript code block (triple backticks)
* An explanation of the syntax using the terms **arrow function**, **parameter**, **code block**, **return statement**, and **call/invoke**.

Below, we've provided an outline for your response but feel free to modify it as you see fit.

### Response

Functions are blocks of code that can be reused in order to complete a task. Functions typically take in an input and return an output based on what was inputted. One way to better visualize how functions work is to think of them as a set of instructions. These instructions are followed in a specific order that result in a desired outcome. They can also be followed as many times as you like to get the same results.

A function declaration in Javascript would look like this:

```js
const getAverage = (...args) => {
    let num = 0;
    for (let i = 0; i < args.length; i++) {
        num += args[i];
    }
    return num / args.length;
}
```

In the code block above, we see a function called get getAverage being declared. First, a variable is created with the name of getAverage. This is then set equal to our parameters that are held within parantheses. After that we put an arrow sign(=>) followed by curly brackets which will contain all of the functions code. This particular function takes in a set of numbers and outputs the average of them. Within the function's block of code, a return statement is used to tell the function what to output.

Here's how we would go about invoking the function in the previous example:

```js
getAverage(1, 5, 9, 10);
// Returns 6.25
```
A function is invoked by using its name followed by a set of parantheses. Within the parantheses, you place in the amount of arguments needed for the function to run. If we were to log the getAverage function to the console with 1, 5, 9 and 10 as the arguments, we would get 6.25.