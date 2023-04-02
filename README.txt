Analysis on Part 3 and 4 - HTML, CSS and JavaScript Code

Sarim Mazhar’s Portfolio
This website will include my information that would be relevant for recruiters and my peers to learn more about me and get to know about my personality.
The HTML and CSS code from A1 and A2 is used for this assignment.

ALL PAGES COMMON CODES
1. <head> element consists of the <title> and the <link> element to set the title of the page and the fav icon.
2. <meta> tag is used to control the accessibility and the content of the page based on the changes in screen sizes.
3. <title>Sarim Mazhar’s Portfolio</title>  display the title on the tabs.
4. <link rel=“icon” href=“My logo.jpg”> displays the personal logo that I made using Paint on windows as the fav icon on the tabs.
5. <style> elements which includes the CSS stylings
6. <img> tag to set the logo of the page (top of the page)
7. <nav> tag to include the nav bar and different links using <a> tags based on the pages.
8. <h3> tag to give a heading/title for the page
9. <br> tag is used to add a break between different section (blank line)

CSS for all pages common code
1. In the html {}, the background colour is set for the html page.
2. In the img.logo {}, the display is set as block and the margins and width id also set for the images.
3. In the nav {}, the display is set as block, the width, padding, alignment, overflow, background colour and the border is set for the nav bar.
4. In the * a {}, the styling is done for all the <a> tags in the page. The display is set to inline, and the padding, text-decoration, colour, and the font-weight is also set for all the <a> tags.  
5. In the nav a:hover {}, hovering effect is set for the <a> tags in the nav bar. The background colour is set for the hover effects.
6. In the h3 {}, the alignment is set to center for the <h3> tags.   


PAGE SPECIFIC CODES

index.html page
<body> tag consists of all the other tags and elements mentioned below.
1. <img> tag is used to include the main picture. It contains a source that links to the picture saved in the folder (relative path) and alt element to give an alternative text for the picture. 
2. <script> tag is included right after the <img> tag. In that script that, I have written the JavaScript code to set a shadow effect to the main picture only if its width is greater than or equal to 450 [1]. 
3. <p> tag is used to add my biography text.
4. <table> tag is used to create a table. It consists of a <caption> tag which sets the heading for the table, the <tr> tag which is the row of the table and inside the <tr> tag there is a <th> tag to include the heading for the first row and also have <td> tags which includes the data for the specific row. 
5. <div> tag is used to create a container and inside that div tag I have three <button> which are used to as colour changers for the table. Each button has an onclick attribute which the routes towards different functions mentioned in the <script> tag below.
6. <script> tag is used to add the JavaScript code. Here three function are created each associated with their respective button. The format and structure  for all the functions are same, except the colour changes. First it asks the user to confirm if they want to change the colour. Is yes then the colour will change, but it they select cancel, the colour will not change. Then I am getting all the <th> tag using the getElementsByTagName) attribute. Using a for loop to loop over all the <th> value, I have added the background colour to it. Same is done for the <td> tags. Except that I have used querySelectorAll() to get the <td> values from the table [2]. 
7. <div> tag again which includes two <a> tags linking to two other pages in the website. 
8. <div> tag which contains a <p> tag to include the Copyright. Copyright symbol is also used in it [3]. 


CSS for index.html
1. img.main{} is used to set the styling for the main picture. The alignment, display, padding, margin, height and width for the image is set.
2. p{} is used to set the alignment, display, margin, padding, line-height and the font size of the text.
3. In the table, td, th {}, the border, height and the alignment is set for all the <table>, <td> and <th> tags.
4. th{} and td{} is used to set the the background colour for the elements.
5. .links{} is used to set the display, alignment and margin for the container with page links.
6. .button{} is used to set the display, padding, margin, border, colour and font for the link buttons.
7. .button:hover{} is used to add a background colour effect for the link buttons.
8. .copyright p{} is used to set the display, margin, alignment and font for the <p> tag inside the copyright class. 
9. .change{} is used to set the top and right position for the change class (buttons with class change)
10. Button{} is used to set the padding of the buttons for colour change. 
11. @media only screen and (min-width: 1000px) and (max-width: 1399px) {} is used to add styling for the tablet format. All the CSS mentioned is added or change accordingly. 
12. @media only screen and (min-width: 1400px) and (max-width: 3500px) {} is used to add styling for the desktop format. All the CSS mentioned is added or change accordingly. 
13. @media only screen and (max-width: 999px) {} is used to add styling for the mobile format. All the CSS mentioned is added or change accordingly. 



gallery.html
1. <ul> tag is used to create an unordered list
2. <li> tags are used to add the images to the gallery.
3. <img> tag is used to include all the pictures. It contains a source that links to the pictures saved in the Assignment folder (relative path) and alt element to give an alternative text for the picture.
4. <script> tag is used to add JavaScript code for the picture. It is used to add borders to an image when it is selected. In the code, I have stored all the gallery items in a variable through getElementById() attribute, and all the images in a variable using getElementsByTagName() attribute. The to loop through all the pictures, I have used a for loop in which I have added an event listener and preventDefault() to prevent the default event to occur if there is an error. I have then used querySelector() on the gallery variable created select the CSS code for .selected. Then I have used the add() method to add the .selected CSS to the selected image. And I have also used a conditional statement to remove the selected CSS from the class [4].
5. <div> tag which includes two <a> tags linking to two other pages in the website. 
6. <div> tag which contains a <p> tag to include the Copyright. Copyright symbol is also used in it [3]. 


CSS for gallery.html
1. #gallery{} is used to set the display, padding, margin and the list-style for the element with an ID gallery.
2. #gallery li{} is used to set the width, height, padding and margin for the <li> tags 
3. #gallery img{} is used to set the width, height and the border for the images in gallery ID.
4. #gallery img:hover{} is used to set the opacity for the images when hovered at.
5. #gallery .selected{} is used to set the border colour for the selected image
6. .links{} is used to set the display, alignment and margin for the container with page links.
7. .button{} is used to set the display, padding, margin, border, colour and font for the link buttons.
8. .button:hover{} is used to add a background colour effect for the link buttons.
9. .copyright p{} is used to set the display, margin, alignment and font for the <p> tag inside the copyright class. 
10. @media only screen and (min-width: 1400px) and (max-width: 3500px) {} is used to add styling for the desktop format. All the CSS mentioned is added or change accordingly. 
11. @media only screen and (min-width: 1000px) and (max-width: 1399px) {} is used to add styling for the tablet format. All the CSS mentioned is added or change accordingly. 
12. @media only screen and (max-width: 999px) {} is used to add styling for the mobile format. All the CSS mentioned is added or change accordingly. 



contact.html
1. <form> element is used to create a form
2. <label> elements are used to provide a label for each field. 
3. <span> is used to add an asterisk with red colour for each label.
4. <input> element is used to take the input for the fields. It includes the type, id, and the placeholder for each of them
5. <textarea> takes a multi-line input for the message text box.
6. <button> is used to add a submit button to the form.
7. <script> tag is used to add the JavaScript code for the form. First I have selected the button using querySelector) attribute. Then I have added an event listener which add preventDefault() to prevent the event in case of any error and then it calls the validateForm() function. The validateForm() function stored all the input values using getElementById() in different variable. Then it validates the form using conditional statements to see if the input value is empty. If it is empty, an alert is shown to the user to add an input and the isValid variable is set to false. When all the inputs are added by the users and invalid is true, then an alert is shown that the form is submitted successfully and the input values are set to empty strings to reset the form values [5]. 
8. <div> tag which includes two <a> tags linking to two other pages in the website. 
9. <div> tag which contains a <p> tag to include the Copyright. Copyright symbol is also used in it [3]. 


CSS for contact.html
1. body::before {} is used to set the background image, size, position, width, height and the opacity for the hero image. Z-index is also set to -1 to have other elements in the page on top of the hero image [6]. 
1. label ~ input {} is used to set the bottom margin, padding, and the width for the <input> tags.
2. textarea {} is used to set the height and the width of the text area. 
3. button {} is used to set the padding and the width for the <button> tags.
4. .links{} is used to set the display, alignment and margin for the container with page links.
5. .button{} is used to set the display, padding, margin, border, colour and font for the link buttons.
6. .button:hover{} is used to add a background colour effect for the link buttons.
7. .copyright p{} is used to set the display, margin, alignment and font for the <p> tag inside the copyright class. 
8. @media only screen and (min-width: 1400px) and (max-width: 3500px) {} is used to add styling for the desktop format. All the CSS mentioned is added or change accordingly. 
9. @media only screen and (min-width: 1000px) and (max-width: 1399px) {} is used to add styling for the tablet format. All the CSS mentioned is added or change accordingly. 
10. @media only screen and (max-width: 999px) {} is used to add styling for the mobile format. All the CSS mentioned is added or change accordingly. 
11. @media only screen and (max-width: 600px) {} is used to add styling for even smaller mobile formats. All the CSS mentioned is added or change accordingly. 






REFERENCES

[1] Style boxShadow Property. W3 Schools. Retrieved April 1, 2023 from https://www.w3schools.com/jsref/prop_style_boxshadow.asp

[2] Changing background color with class. Code Cademy. Retrieved April 1, 2023 form https://discuss.codecademy.com/t/changing-background-color-with-class/385183

[3] HTML Symbols. W3 Schools. Retrieved April 1, 2023 from https://www.w3schools.com/html/html_symbols.asp

[4] 2021. How to add and remove a CSS class from multiple elements with . Go Make Things. Retrieved April 1, 2023 from https://gomakethings.com/how-to-add-and-remove-a-css-class-from-multiple-elements-with-vanilla-javascript/

[5] JavaScript Forms. W3 Schools. Retrieved April 1, 2023 from https://www.w3schools.com/js/js_validation.asp

[6] CSS z-index Property. W3 Schools. Retrieved April 1, 2023 https://www.w3schools.com/cssref/pr_pos_z-index.php
