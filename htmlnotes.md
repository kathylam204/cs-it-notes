# HTML

## HTML Defined:
- A markup language used to structure and present content on the web.
- Provides a framework for creating web pages and applications.
- Defines elements for text, images, links, forms, and multimedia.
- Facilitates user interaction with web content.

## Key Elements:
- Anchor Element (<a>): Creates hyperlinks to other webpages, files, or sections of the same page.
- Input Element (<input>): Renders various types of input fields such as text boxes, checkboxes, radio buttons, and buttons; its functionality is determined by the type attribute.
- Form Element (<form>): Collects user input for submission to a server.
- Label Element (<label>): Associates descriptive text with specific input fields for accessibility.
- Semantic Elements: Introduced to provide meaning to the markup structure and enhance accessibility (e.g., <header>, <footer>, <article>, <section>, <aside>).

## Input Types:
- Text Input: <input type="text"> allows single-line text input.
- Password Input: <input type="password"> masks sensitive input.
- Number Input: <input type="number"> restricts input to numeric values and can include attributes such as min, max, step.
- Checkbox Input: <input type="checkbox"> allows selection of one or more options.
- Radio Button: <input type="radio"> enables single selection within a group.
- Range Input: <input type="range"> provides a slider for selecting numeric values.
- File Upload: <input type="file"> allows users to upload files.
- Dropdown: <select> creates a dropdown list with <option> elements for choices.

## Common Attributes:
- name: Defines a key in key-value pairs for form submission.
- value: Specifies the default value to be submitted.
- required: Indicates that the field must be filled before submission.
- maxlength & minlength: Sets constraints on the length of text fields.
- max & min: Sets limits on numeric fields.
- pattern: Uses a regular expression for input validation.
- placeholder: Provides guidance on what to enter in an input field.

## Semantic HTML Elements:
- <header>: Defines the header section of a document.
- <nav>: Contains navigation links.
- <main>: Encloses the primary content of the document.
- <footer>: Contains the footer section of the page.
- <article>: Represents self-contained content, such as a news article.
- <section>: Groups related content, usually with a heading.
- <aside>: Contains supplementary content related to the main content.
- <figure> and <figcaption>: Encapsulates media and its description.

## Media Elements:
- <video>: Embeds video content in the page.
- <audio>: Embeds audio content.
- <embed>: Integrates external media sources, such as images or interactive content.

## Form Submission:
### Forms utilize:
- action: Specifies the destination URL for the submitted data.
- method: Dictates the HTTP method used (GET, POST, etc.).

## Validation:
- HTML includes built-in validation features for form inputs:
- Required fields must contain user input.
- Maximum and minimum values enforce constraints on numeric inputs.
- Pattern matching checks for specific input formats.
- Length constraints apply to text inputs to limit character count.

## HTML Form Validators:
- HTML forms support various validators, such as:
- Minimum and maximum values for number inputs.
- Minimum and maximum length for string inputs.
- Pattern validation using regular expressions.

## Additional Concepts:
- Submit Button: <input type="submit"> creates a button to submit the form.
- Datalist for Autocomplete: <datalist> provides a list of predefined options for <input> fields.

## Example Input Types:
### Number Input:
- <input type="number" name="balance" />
### Text Input:
- <input type="text" name="username">
### Password Input:
- <input type="password" name="password" required>
### Range Input:
- <input type="range" name="volume" min="0" max="100">
### Checkbox Input:
- <input type="checkbox" name="subscribe" value="newsletter"> Subscribe to newsletter
### Radio Button:
- <input name="delivery_option" type="radio" value="pickup" /> Pickup\
- <input name="delivery_option" type="radio" value="delivery" /> Delivery
### Dropdown:
- <select name="rental-option">
- <option value="small">Small</option>
- <option value="family">Family Sedan</option>
- <option value="lux">Luxury</option>
- </select>
### File Upload:
- <input type="file" name="upload">
### Example of Datalist:
- <input list="ide" />
- <datalist id="ide">
- <option value="Visual Studio Code" />
- <option value="Atom" />
- <option value="Sublime Text" />
- </datalist>
### Example of Form:
- <form action="/submit" method="POST">
- <label for="username">Username:</label>
- <input type="text" name="username" required>
- <label for="password">Password:</label>
- <input type="password" name="password" required>   
- <input type="submit" value="Submit">
- </form>
