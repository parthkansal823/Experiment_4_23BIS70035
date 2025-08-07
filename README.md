# 📝 Live Character Counter for Text Area

## 🎯 Objective

Create a simple feature that displays a **live character count** as the user types in a `<textarea>`. This task helps you practice **real-time event handling** and **dynamic content updates** to improve user interaction and feedback.


## 📋 Task Description

Build a web page that includes:

- A **textarea** where the user can input text.
- A **live character counter** displayed below or beside the textarea.

### ✅ Functionality Requirements

- The counter should:
  - Update **immediately** as the user types or deletes content.
  - Show the **current number of characters** entered.
  - Provide **clear and instant feedback**.

> This task focuses on DOM manipulation using JavaScript and reinforces user-centric UI behavior.

## 📸 Screenshots
### Code – HTML5  
[View Code](Experiment.html)

### Code – CSS  
```
.container {
    border: 1px solid black;
    padding: 10px;
    font-family: Arial, Helvetica, sans-serif;
    max-width: 500px;
}

textarea {
    width: 100%;
    height: 80px;
    font-size: 16px;
    padding: 8px;
    box-sizing: border-box;
    margin-bottom: 8px;
}

.counter {
    font-size: 1.1em;
    margin-top: 4px;
}

.counter b {
    font-weight: bold;
}
```

### Code – JavaScript  
```javascript
const textarea = document.getElementById('textinput');
const counter = document.getElementById('charCount');

textarea.addEventListener('input', () => {
    counter.textContent = textarea.value.length;
});
```

### Output
![Alt Text](result1.png)
![Alt Text](result2.png)

## Learning Outcome
- Gain experience with real-time **DOM event handling**.
- Practice **updating UI dynamically** with JavaScript.
- Improve **user interaction feedback** using simple logic.
