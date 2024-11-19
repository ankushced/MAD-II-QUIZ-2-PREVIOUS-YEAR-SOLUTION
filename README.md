# MAD-II-QUIZ-2-PREVIOUS-YEAR-SOLUTION
Let's begin with the first question listed in the document.

---

### Question 1 (Question 356 from the document):
**Context:**  
This is a multiple-choice question that references an HTML document. The question likely involves understanding DOM structure and browser behavior when interacting with a specific element in the HTML, particularly a table cell.

**Question:**  
Suppose you open the `index.html` file in a browser and click on the table cell with the text "Abhishek." What will be the correct sequence of outputs?

**Explanation and Answer:**  
This type of question requires understanding how event handling works in HTML and JavaScript, particularly within table cells.

---

#### Detailed Explanation:
1. **Event Flow in JavaScript (Bubbling and Capturing):**  
   - **Bubbling:** Events propagate from the deepest element (clicked element) to the parent and then to the document. For example, clicking on a `<td>` will bubble the event to `<tr>`, `<table>`, and then the document.
   - **Capturing (or Tunneling):** Events propagate from the document to the deepest target element. Less commonly used.

2. **Structure of the HTML Document:**  
   - The document likely includes a table where cells (`<td>`) have event listeners.  
   - Clicking "Abhishek" triggers the `onclick` event for the `<td>` containing "Abhishek."

3. **Output Sequence:**  
   - The sequence depends on:
     - The specific event listeners added to the elements.
     - The order of propagation (bubbling or capturing).

---

#### Related Concepts:
- **JavaScript Event Listeners:**
  - **`addEventListener()` Method:** Allows adding multiple listeners to an element.
  - Example:
    ```javascript
    document.querySelector('td').addEventListener('click', function() {
        console.log('Cell clicked!');
    });
    ```

- **DOM Hierarchy:** Understanding parent-child relationships in the HTML structure is crucial for predicting event propagation.

- **Preventing Default Behavior:** Use `event.preventDefault()` to stop default actions (like a form submission).

---

If the solution in the document provided a specific sequence of outputs, it aligns with how events are set up in the code.

Would you like me to move to the next question, or is there something you'd like to clarify about this one?
