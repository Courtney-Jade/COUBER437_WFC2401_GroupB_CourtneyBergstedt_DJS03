# Book Connect

##  Original Code Structure
The original structure of the code was repetitive. The theme application logic was scattered throughout the code and the event listeners was attached within the main execution flow of the code.

## My Task

1. **Code Analysis**: Start by understanding the current implementation of the "Book Connect" application, including its HTML structure and JavaScript functionality.
2. **Plan Refactoring**: Identify sections of the code that can be made more abstract and modular. Look for patterns and repetitive code that can be simplified.
3. **Implement Abstraction**:
   - **Objects**: Define objects to represent key elements of the application, such as books, authors, and genres. Utilise the provided data (e.g., `authors`, `genres`, `books`) to populate these objects.
   - **Functions**: Create functions that handle repetitive tasks, such as rendering the book list, handling user interactions, and applying filters.
4. **Enhance Functionality**: Ensure that the application remains fully functional after refactoring. Test all features to confirm that users can still search, filter, and view books as intended.
5. **Documentation and Comments**: Throughout the refactoring process, document your code. Provide comments that explain the purpose and functionality of objects and functions.
6. **Adherence to Styleguides**: Ensure your code follows JavaScript and HTML coding standards and best practices for readability and maintainability.

## Changes Made
1. Introduced the 'app' object to manage application state. Line 4
2. Abstracted book list rendering into 'renderBookList'. Line 13
3. Abstracted dropdown creation into 'createDropdownOptions'. Line 32
4. Consolidated event listener setup into setupEventListeners. Line 59
5. Encapsulated theme application logic into applyTheme. Line 48
6. Centralized book filtering logic in filterBooks. Line 109
7. Encapsulated book detail display in showBookDetails. Line 131

### Challenges
The challenges I found was identifying all the repetitive code patterns and decide on how to incorporate abstraction into the code by refactoring it.I also had to make sure that when refactoring the code that the app was still functional.