# HTML Forms

When a user submits a form on the computer, the name of each **form control** is sent to the server along with the value the user enters or selects. The server then processes that information using a programming language and creates a new page to send back to the user. 

**Form controls** collect information from websites.  There are several types of form controls in the form of an `input`, such as:
- text input
- password input
- text area
- radio buttons
- checkboxes
- dropdown boxes
- submit buttons
- image buttons
- file upload

The server uses key/value pairs to know which piece of inputted data corresponds with which form element

```
username = Ivy
```

Each form control lives inside a `<form>` element and requires an **action attribute** and **method**:
- action attribute: the URL for the page the server will receive the information on
- method: either GET or POST

```
<form action="http://www.example.com/subscribe.php" method="get">
<p>This is where the form controls will appear.
</p> </form>
```

Forms can also have buttons, labels, fieldsets, legends, etc.

# HTML attributes for forms, lists, and tables

How to style.. 

Lists:
- `list-style-type`
- `list-style-image`
- `list-style-position`

Tables:
- give cells padding
- distinguish between headings
- shade alternate rows
- put a border around `empty-cells`
- border spacing
- `border-collapse`

Forms:
- style border or background color
- use pseudo-class `:hover`
- style submit buttons
- style the legend
- align elements 
- change curser style