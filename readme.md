1. What is the difference between getElementById, getElementsByClassName, and      querySelector / querySelectorAll?
Ans:
getElementById returns a single element since there is only one Id in a file, 
getElementByClassName returns multiple elements because of having multiple Class names,
querySelector represents the first matching element, and lastly
querySelectorAll gives all matching elements.

2. How do you create and insert a new element into the DOM?
Ans:
Usually we create and insert a new element into the DOM following 3 steps like,
        1. Create 
        2. Customize 
        3. Insert
    const newParagraph = document.createElement("p");
    newParagraph.textContent = "Hello World";
    document.body.appendChild(newParagraph);

3. What is Event Bubbling and how does it work?
Ans:
Event bubbling is the process where an event starts from the target element and then bubbles up through its ancestors.

    <div id="parent">
  <button id="child">Click Me</button>
</div>

document.getElementById("child").addEventListener("click", function(){
  console.log("Child clicked");
});

document.getElementById("parent").addEventListener("click", function(){
  console.log("Parent clicked");
});


