# Module 2 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

*Note: any topics from the first assessment should be reviewed in addition to the questions below!*

## CSS

### Questions

1. What is the box model?
A: A box that wraps around an html element that is made up of border, padding, and margin.

2. What is the difference between block and inline elements?

A: Block elements have display values set to bloc, which means they have a set width and height. Inline elements don't have defined width/height, and won't start a new paragraph automatically. 

3. What is responsive design?
Using HTML and CSS to make a website look great on any screen. 

4. Which selector is more specific, a tag selector or class selector?
A: tag selector 

5. What does `box-sizing` do?
A: it allows you to resize an HTML element as a group: When resizing, you are also resizing padding and border.

6. What's the difference between `relative` and `absolute` positioning?

### Exercises

1. Write a CSS rule to turn the background color of the link with the `.btn` class blue on hover:

  ```html
  <a href="#" class="btn">Learn more</a>
  ```
ANSWER: 
.btn:hover {
  background-color: blue; 
}

2. Write a CSS rule to give the `.container` a maximum width of `980px` when the browser window is wider than `1200px`:

  ```html
  <div class="container">
    <h1>I'm a heading!</h1>
  </div>
  ```

3. Which text would be red in the following example?

  ```html
  <style>
    section p:last-child {
      color: red;
    }
  </style>

  <section>
    <p>First paragraph</p>
    <p>Second paragraph</p>
    <p>Third paragraph</p>
  </section>
  <section>
    <p>First paragraph</p>
    <p>Second paragraph</p>
    <p>Third paragraph</p>
  </section>
  ```
ANSWER: "Third Paragraph"

4. Open this [JSBin](http://jsbin.com/qigiwuhepe/1/edit?html,css,output). Write a CSS rule using floats to make the HTML sample into a four column layout. Paste your udpated link below.

## JavaScript

### Questions

1. What is a callback?
When you force a function to wait for a separate function to fire.

### Exercises

1. Write a function `filterLongWords()` that takes an array of words and an integer `num` and returns the array of words that are longer than `num`.

ANSWER: 

function filterLongWords(array, num) {
  
  if (array.length > num) {
   return array; 
  }
  
  else {
    console.log("Sorry, nothing was bigger than num");
  }
}

filterLongWords("alphamatrazc", 4); 



2. Write a function `charFreq()` that takes a string and builds a frequency listing of the characters contained in it. Represent the frequency listing as a Javascript object. Try it with something like `charFreq("abbabcbdbabdbdbabababcbcbab")`.

ANSWER:
function charFreq(string) {
  var freq = {};

  for (var i=0; i<string.length; i++) {
     var characters = string.charAt(i);
     
     if(freq[characters]) {
       freq[characters]++;
     }
     else  {

       freq[characters] = 1; 
     }
  }
  return freq; 

};

## DOM Scripting

### Questions

1. What does DOM stand for and what is it?
ANSWER:
Document Object Model
It's the browser's internal representation of a webpage. 

### Exercises

1. Write a JavaScript statement that finds the element with the ID, `next`, and saves it to a variable called `nextButton`:

  ```html
  <a href="#" id="next" class="btn">Next</a>
  ```
  ANSWER:
 var nextButton = .document.GetElementbyID("next");
  

2. Write another line that updates the text of `nextButton` to `"Next image"`.

ANSWER:
  var x = getElementByClassName("Next");
  x[0].innerHTML = "Next Image";

3. Write another line that adds a click event listener to `nextButton` so that when it's clicked the browser alerts `"Next image coming up."`.

document.getElementbyID("btn").addEventListener("click", "Next image coming up.");

## jQuery

### Questions

1. What is a JavaScript library and why do we use them?
2. What is jQuery for?

### Exercises

1. Write a statement to select all elements with the `.btn` class using a jQuery selector and save them to a variable called `buttons`:

  ```html
  <a href="#" id="next" class="btn">Next</a>
  <a href="#" id="beginning" class="btn">Beginning</a>
  <a href="#" id="previous" class="btn">Previous</a>
  ```

2. Write another line that adds a click event to the buttons that logs `'click'` to the console when the button is clicked. Use the jQuery syntax.

## Angular

### Questions

1. How is a framework different than a library?
2. What is a controller?
3. What is a view?
4. What is a single page application?
5. What is a directive in Angular?

## Git

### Exercises

1. Write a command to create a new branch called `bug-fix`.
2. If you're on the `master` branch, write a command to merge a branch called `bug-fix` into the `master` branch.
