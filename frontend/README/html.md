# HTML
 - html -hypertext markup language.
 - it gives the structure for the web page.
 - HTML elements tell the browser how to display the content.
 ## HyperText
    - This means text with links.
    - Stuff you can click and jump to another page, section, or site.
 ## Markup
    - Markup = adding tags to text to describe what it is
    - Not how it looks, but what it means
    - You “mark up” plain text with labels (tags) so a computer/browser knows:
  - this is a heading
  - this is a paragraph
  - this is a link
  - this is an image

# Tags
     <h1> </h1> here <h1> --> opening tag </h2> --> closing tag

     - from h1 to h6 there 6 tags from 1 to 6 the size keep on decreasing
     -  you can also write the sentence without tag it wil also get printed.

     e.g <h2> hello </h2>
     
 ## paragraph tag
     - <p>lorem epsom blah blah </p>

 ## anchor tag
     - <a></a> --->The anchor tag is used to create hyperlinks.

     - here an attribute called href is used to create the hyperlink 

     - attribute-An attribute is extra information you add to an HTML tag to define its behavior or properties.
       
    - tagname → the HTML tag (<a>, <img>, <p>, etc.)

    - attribute → the property you want to set (href, src, alt, etc.)

    - value → the specific setting for that attribute
  
### HTML `<img>` Tag

- `<img>` is used to display images on a web page.
- It is a self-closing tag (no closing tag needed).

#### Common Attributes
- `src` → source of the image (path or URL)  
- `alt` → alternative text if image doesn’t load  
- `width` → width of the image  
- `height` → height of the image  
- `title` → tooltip text on hover  

#### Example
```html
<img src="cat.jpg" alt="Cute cat" width="200" height="150" title="My Cat">



### HTML LIST
    - there are two types of lists ordered  and unordered 
    - ordered one gives in 1 2 3 .. order or any thing we want in roman order 
      <ol>
        <li> Apple </li>
        <li> Banana </li>
      </ol>
    - unorder gives in bulletin or our desired forms 
      <ul>
        <li> Apple </li>
        <li> Banana </li>
      </ul>

## iframe
     - means bringing another website into our website!
     <iframe src="link"></iframe>

## hr tag
     - draws a  horizontal line.

## br tag
     - it used to break that line and perform the next action in next line.

##link tag
    ### `<link>` Tag and `rel` Attribute

- `<link>` is used to connect an HTML document with external resources.
- It is placed inside the `<head>` section.
- It is a self-closing tag and is not clickable.

#### `rel` Attribute
- `rel` stands for relationship.
- It tells the browser what kind of file is being linked and how to use it.

#### Example
```html
<link rel="stylesheet" href="styles.css">

     




##  HTML BOILERPLATE

    - Boilerplate = standard reusable code written before the main logic

    //boilerplate
        <!DOCTYPE html>
        <html>
        <head>
          <title>Page</title>
         </head>
         <body>
         </body>
        </html>



## HTML TABLE
   -boilerplate
   <table border="1"> <!--- border is an attribute which creates an border of 1(light shade)-->
    <th> Name </th> ---> table heading gives in bold color
    <tr> 
      <td> </td> ---> column(table data)
    </tr> ---> table row
    <table>




Structured format 
<table>
  <caption>Student Marks</caption> --> gives a little caption

  <thead>
    <tr>
      <th>Name</th>
      <th>Marks</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>Shivv</td>
      <td>98</td>
    </tr>
  </tbody>

  <tfoot>
    <tr>
      <td>Total</td>
      <td>98</td>
    </tr>
  </tfoot>
</table>

  
## FORM

  <form>
    Name:<input type="text">
    Age:<input type="number">
    <input type="submit">
    <input type="reset">
    </form>

    - <input> --> gets the input
    - type inside the inside decides what type of input we should get if text we can write anything (text is default if type not given) if number we can only type number as input.
     
     - using just the form doesnt gives the better alignment hence use table inside form (combine table and form)

form and table combined

<form>
    <table>
        <tr>
            <th>Name:</th> <td><input type="text" placeholder="Enter your Name"></td>
        </tr> 
        <tr>
            <th>Age:</th> <td><input type="number" placeholder="Enter your age"></td>
        </tr>
        <tr>
            <th>Address:</th> <td><input type="text" placeholder="Enter your address"></td>
        </tr>
        <tr>
            <th>Department:</th> 
            <td>
                <select>
                    <option> Java </option>
                    <option> Python</option>
                    <option> C++ </option>
                </select>
            </td>
        </tr>
        <tr>
            <th></th> <td><input type="submit"></td>
        </tr>
    </table>
</form>




