# Module 1 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

## HTML

### Questions

1. What is HTML and what is it used for? 
ANSWER: hypertext markup language that are placed inside a file to edit words/text on a website. 

2. What is the difference between an ID and a class?
NEED TO STUDY

3. What does it mean to write "semantic" HTML?
To write code that modifies or defines the meaning of content on a webpage (not just the look of a page)

### Exercises

1. Write a paragraph tag with a class of "highlight" and content "Watch out!".

<p class="highlight">Watch Out!</p>

2. Write an HTML image tag to show an image called `profile-picture.jpg`.

<img src="profile-picture.jpg">

3. Write a link tag that links to http://google.com.
<a href = "http://www.google.com">Take me to Google</a>

5. Write an complete standard HTML document outline (including a DOCTYPE, and `<html>`, `<head>`, and `<body>` tags).

<!DOCTYPE html>
<html>
  <head>
  <head/>
  <body>
    <p></p>
  </body>
</html>

6. Inside of the code for the previous exercise, write the appropriate tag to link to a script file called `main.js`.

<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" type=text/css href=main.js>
  <head/>
  <body>
    <p></p>
  </body>
</html>

7. Inside of the code for the previous exercise, write the appropriate tag to link to a stylesheet file called `main.css`.

<!DOCTYPE html>
<html>
  <head>
  <style type ="main.js">
  <head/>
  <body>
    <p></p>
  </body>
</html>

8. Write a numbered list in HTML and list three of your favorite books.

<body>
    <ul>
      <li>The Season of the Witch</li>
      <li> Woman in White</li>
      <li>The Turn of the Screw</li>
    </ul>
    
9. Fix the indentation of the following HTML sample:

  ```html
  <div>
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
    </ul>
  </div>
  ```

## CSS

### Questions

1. What is CSS and what is it used for?
ANSWER:
CSS is a language used to styles HMTL language and set its look.

2. What is the CSS box model?
It controls the spacing and padding between boxes of each tag. 

3. What's the difference between margin and padding?
Padding is the layer outside of the content.
Margin is outside of the border, whic it oustside of the padding.

### Exercises

1. Write a CSS rule to make the text of all `h1` tags red.

h1 {
 text-decoration-color:red;
}

2. Write a CSS rule to make the background color of the link with `class="btn"` blue:

  ```html
  <a href="#" class="btn">Learn more</a>
  ```

3. Write a CSS rule to give the first paragraph in the following HTML a font size of `20px`, but not the second paragraph.

  ```html
  <header class="jumbotron">
    <p>Hello, World!</p>
  </header>

  <p>Welcome to this awesome website!</p>
  ```

## JavaScript

### Questions

1. What is a function? What are they used for?
2. What is the difference between `==` and `===`?
3. What is the difference between global and local scope variables?
4. What is a boolean value?
5. What is an array?

### Exercises

1. Write a line that declares a variable called `myName` and set its value to your name.
var myName = "Ann Murray";

2. Write a loop that logs the numbers 1 through 10 to the console.

for (var num = 0; num < 11; num++) 
{
console.log(num)
}

3. Translate the following pseudocode into JavaScript: if `score` is greater than `3` and `lives` is greater than `0`, alert "You win!".

function winning(score,lives)
{
  if (score > 3 && lives > 0);  
  { 
    alert("You win!"); 
  }
};
winning(4,1);

4. Write a function `sayHello` that takes one argument, a name, and logs "Hello, <name>!" to the console. Then, call the function below the function definition and pass in your name as the argument.

var name = "Ann"

function sayHello() 
{
  console.log("Hello, " + name + "!");
}
sayHello(name);

5. What would the following script log to the console?

  ```javascript
  var currentSong = "Call Me Maybe";

  function setSong(song) {
    currentSong = song;
  }

  setSong("Friday, Friday");

  console.log(currentSong);
  ```

6. What would the following script log to the console?

  ```javascript
  var add = function(a, b) {
    return a + b;
  }

  var result = add(3, 7);

  console.log(result);
  ```

7. What would the following script log to the console?

  ```javascript
  var helloGoodbye = function(name) {
    return sayHello(name) + " " + sayGoodbye(name);
  }

  var sayHello = function(name) {
    return "Hello " + name " !";
  }

  var sayGoodbye = function(name) {
    return "Goodbye " + name " !";
  }

  console.log(helloGoodbye("Sarah"));
  ```

8. Write a function `findLongestWord()` that takes an array of words and returns the length of the longest one.

function findLongestWord()
{
  var words = ["Ann", "Benny", "Murray"];
  var largestnumber = 0;
  var maxword; 
  
  for (var i = 0; i < words.length; i++) 
  {
    if (words[i].length > largestnumber) 
    {
    maxword = words[i];
    } 
  }
   console.log(maxword);
}

findLongestWord();

9. Define a function `sum()` that sums all the numbers in an array of numbers. For example, `sum([1,2,3,4])` should return 10.

function sum()
{
  amount = 0;
  
 for(var i=0; i<arguments.length; i++)
    {
      amount = amount + arguments[i];
    }
  console.log("the number is: " + amount);
};

sum(1,1,1,1,1,1);

10. Write a function that takes a character (i.e. a string of length 1) and returns true if it is a vowel, false otherwise.
11. Write the correct line to make `"Woof!"` show up in the console based on this script:

  ```javascript
  var pet = {
    name: "Charles",
    goodDog: true,
    speak: function() {
      console.log("Woof!");
    }
  };
  ```

12. Using the same script as above, write the correct line to log the dog's name to the console.

## Command Line

### Questions

1. What is the command line and what is it used for?
2. What does the command `ls` do?
3. What does the command `pwd` do?
4. What does the following command do: `cd my-cool-project`

### Exercises

1. Write the command to make a new directory called "my-cool-project".
2. Write the command to create a file called "index.html".
3. Write the command to delete a file called "main.css".

## Git

### Questions

1. What is Git and what is it used for?
2. What's the difference between a local repository and a remote repository?

### Exercises

1. Write the command that you would use to create a new local Git repository.
2. Write the command to stage a file called `index.html` to be committed.
3. Write the command to view the current status of the git repository.
