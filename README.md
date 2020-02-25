# Foundation for Logic in JavaScript Using Math, Variables and Comparisons

We now move away from using coding to simply add interactivity to a website. Instead, we harness JavaScript's ability to calculate and to compare -- all foundations for programming logic.

## Hello JavaScript Console

Visit [this blank page.](http://www.this-page-intentionally-left-blank.org/)

Open the browser's JavaScript console by using **command**-**option**-**J** (⌘ ⌥ J). Use Chrome!

Click on console

Let's do some simple math:

![](/img/basicmath.png)

You can also group:

![](/img/grouping.png)

Remember [PEMDAS](https://www.mathsisfun.com/operation-order-pemdas.html)

But using JavaScript as a calculator is not the goal. Instead we want a way to hold numbers and other information that we can manipulate on the fly.

## Variables at Work

Back in the console, type `let x = 1000;` and hit enter.

In the next line, type x

You should see "1000".

Now type, `let y = 1100;` and hit enter.

Now type y

You should see "1100".

Now for something that neither HTML or CSS can do: Math.

Type `x — y` into the console.

You should get -100.

![](/img/let-variables.png)

## More on Variables

Variables are placeholders for values. They can be any of the following:

-   **Numbers**
-   **Strings**, that are made up of letter, words, sentences, etc.
-   **Placeholders**, that receive their value from inputs, computations or concatenation of other variables.
-   **Arrays**, that holds a multiple values in one variable.
-   **Objects**, variables that hold interrelated data or info. (more on this in the advanced course!).
-   **Functions**, that you can call in one or more places in your code (more on this at some point this semester!).

## How Might We Use Variables in Journalistic Interactives?

-   Store large amounts of organized information and pull out key info based on user interaction. (<http://nynumbers.nycitynewsservice.com/gun-violence/> \| <http://graphics.wsj.com/childcost/>)
-   Take user input, run it through a formula and store the result to be used later. (<https://sandeepmj.github.io/syria/>
-   Taking in user inputs and return some information (<https://www.nytimes.com/interactive/2014/05/20/dining/what-are-you-drinking.html>)

### Why use Variables?

-   **Clarity** — you can assign meaningful names to variables.
-   **Reusability** — you can use the same variable in different places in your code.
-   **Time saver** — you can change its value in one place and the new value is called on throughout your code
-   **Placeholder** — a variable can be empty until some event or user action or input gives it a value.

### Naming Variables

This semester we will mostly work with two types of variables:
**let** — is a type of variable that can change values.
**const** — is the type of variable where the value is constant.

The idea is to give meaningful names so you aren't confused by what they stand for. Apart from that, here are some basic rules:

-   They ARE case sensitive.
-   Cannot begin with numbers.
-   Make them unique (just like IDs, you should only have ONE variable with a particular name).
-   No spaces between words, instead use underscores, hyphens or camelCase (`let myCamelCaseExample`).
-   Don't use any JavaScript [reserved words](http://www.w3schools.com/js/js_reserved.asp).
-   Think of code as story. Each variable is like a character/actor. Naming each in a relevant way such makes the narrative (the code) easier to follow.
-   Keep the variables short but make sure they make sense.
-   Don't integrate values into the name of a variable. For example, for drinking age, `let legal21` might work. But what if you expand your piece internationally? Or what if the legal age changes? Making it `let legalDrinkingAge` is more adaptable.

Our example where we had `let x = 1000` and `let y = 1100`. What if those values stand for someone's paycheck and expenses. As our code gets longer, we'd forget what `x` and `y` stand for. Instead, we provide meaningful variables:

 ![](/img/monthlyexpenses.png)

-   You can also declare a variable and assign a value based on a computation at one time:

    ![](/img/assignlet.png)

You get the same results but you won't be confused by these variables later as you would be by x and y.

<!-- ### Global v. Local Scope

-   Local variables only work within the function they are in.

-   Global variables can be used by multiple functions on the page.

More on this later in the semester. -->

### Declaring a Variable

-   For a number, you simply type `let someNumberDog = 123;`

-   For a string, you type `let someStringCat = "Some string of letters, words, etc.";`

-   Strings must be contained within either `'Single Quotes'` or `"Double Quotes"`. You can't mix and match.

-   You can also declare a variable but assign it a value later based on a computation or some input (age, name, etc.). You simply type `let somePlaceholderDogName;` to declare a variable with no value.

<!-- -   Declaring all variables at the start is good practice. In the following example, we create global variables:

![](/img/declarations.png) -->

### Exercise One (a few minutes)

Create variables for the following:

-   The numeral 5 as a number.
-   The number 4 as a string

Add the two variables together. What do you get?

Flip the order of adding them together. What do you get?

### What Type of Variable?

![](/img/typeof.png)

<!-- ![](/img/mag-glass.jpg)What's happening?

![](/img/monthly.png) -->

### Exercise Two (10 minutes)

Create three variables that hold _real world_ numbers (cost of groceries, criminal justice numbers, etc) and do a _real world_ mathematical operation on them in the console.

### Escaping Special Characters

Type the following into your console:

`let testString = ""He could not find his keys," the inspector said.";`

`let testString = 'It's time to sleep.';`

![](/img/string-quotes-error.png)

You get an error. Why?

You'll recall that strings in a variable have to be contained within either `'Single Quotes'` or `"Double Quotes"`. The problem occurs when a `"Double Quotes"` string itself contains a quotation. Or a `'Single Quotes'` string has a contraction that uses an apostrophe.

We get around this situation by using the `\ escape character.`

Try it. Type the following into your console:

`let testString = "\"He could not find his keys,\" the inspector said."`

`let testString = 'It\'s time to sleep.';`

Now the strings work and you see either the quotation or the apostrophe.

![](/img/escaping.png)

### Concatenation

The plus sign `+` joins two string variables together.

Remember, if you put a `+` between two variables that hold numbers, it will add the two numbers together.

### Exercise Three (10 minutes)

Create variables for each of the following lines (those are quote marks):

-   "It's been
-   a hard days night
-   and I've been working like a dog."

Now create a variable that combines previous variables to create a complete sentence.

HINT: strings can be added together.

<!--
### Arrays

Often you'll want one variable to hold multiple values. These special variables are called "arrays" and give you great versatility.

Let's try this simple array. We give the array a name and some values. We can use the **`.length`** method to see how many values are in the array.

You can retrieve values by typing `nameOfArray[indexNumber]` where the index number is the position in the list. In computing, 0 (zero) is always the first position in an index.

![](/img/arrayintro.png)

You can even add more values to an array using the  **`.push()`** method

![](/img/arraypush.png)

Why would you need an array?

For example, let's say you are building an interactive that explores the impact of massive budget cuts on a number of U.S. government agencies. Instead of creating a variable for each agency, we can place them all in an `Array`.

You declare arrays the same way using `let =` or `const =` but then use place values in quotes within square brackets.

For those of you who know some Python, an `array` is similar to a `list`.

`let agenciesCuts = ['EPA', "NEA", 'State Dept.', 'DOJ — Civil Rights Division', " Consumer Protection Agency"];`

You retrieve values by typing `agenciesCuts[indexNumber]`

### Objects

Objects are variables that can hold interrelated data.

![](/img/menu.png)

If you expand one of the triangles you can see the index position:

![](/img/menu-expanded.png)

We aren't likely do much more with objects this semester, but are incredibly powerful, flexible and complex. Objects are what make JavaScript an "object-oriented" language. -->

## Comparison Operators

JavaScript allows us to make comparison which then allows us to take an action. For example, if a user is paying more than 35 percent of his or her income on rent, we can tell them they are overpaying.

You've seen some of these operators before:

-   `5 > 3` or 5 is greater than 3.
-   `4 < 8` or 4 is less than 8.

Where it gets a little stanger is for **equal** and **not equal**. Because we use `=` to assign value to a variable, we have to use `==` to denote equality and `!=` for inequality

Here's a [complete list of comparison operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#Comparison_operators)

### Logical Operators

Logical Operators simply allow you to compare relationships or logic between various variables-- like **and** and **or**. The logic for "and" is written as `&&` and the logic for "or" is written as `||`. Here's a [full list of logical operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#Logical_operators).

![](/img/comparison.png)

### So What?

At this point you might be wondering, yeah so what?

Here's what:

Imagine an interactive that does different things based on user input. For example, **`if`** someone someone's monthly rent is more than 35 percent of their monthly income, the interactive tells them they are overpaying, **`else`** it tells them they are paying the right amount.

JavaScript actually has powerful **`if`** **`else`** conditional statements for such purposes.

### Homework

Declare the variables that you might use to create an interactive about the following **made up** situation:

A refugee inputs the number of members in their family. Based on that number, you tell them how much money they will receive as assistance based on the following: Each family member is given a one-time grant of $1,000  in 2018. Refugee families arriving in 2019 might get more or less depending on the State Department funding priorities. You need to know if the head of household speaks English. The refugee (and their family members) will be settled in the New York City where there are 5 NGOs that might help them. The five NGOs are "Help Unlimited", "New Start", "Better Tomorrow", "Home Safe" and "New Home". The monthly estimated expenses are as follows. Just one person will be $800. A couple will be $950; A family of three will be $1000. A family of four will be $1100. A family of five and above will be a fixed $1200.  

Create a .js file and declare relevant variables.

  \*\*Due: Friday 5pm as a link to a GitHub repo that you have created AND then fill out this form (<https://goo.gl/forms/GhOnnOdqlUReWRou2>).
