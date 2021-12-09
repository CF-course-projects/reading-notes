
<p>Form Controls: There are different types of form controls to collect info</p>
<ul>
<li>Adding text: <ul>
<li>Text input: used for single line of text like emails and names</li>
<li>Password input: like a text input but masks the characters</li>
<li>Text area: used for multiline text input</li>
</ul></li>
<li>Making Choices<ul>
<li>Radio buttons: used to create a selection of multiple options (pick one)</li>
<li>Checkboxes: create a selection of multiple options (can pick multiple)</li>
<li>Drop-down boxes: create a selection of multiple options in list form (pick one)</li>
</ul></li>
<li>Submitting Forms: <ul>
<li>Submit buttons: to submit data from your form to another web page</li>
<li>Image buttons: like submit buttons but you can use an image</li>
<li>File upload: users can upload files to the site</li>
</ul></li>
</ul>
<p>Forms use key-value pairs to store user-inputted data <br> 
Note: NEVER change the name of a form control unless you know the code will understand the new key value</p>
<p></p><br>
<p>Form structure and Elements</p>
<ul>
<li>form: creates the body of the form; every form tag must have an action attribute. The value of the action attribute is the URL of the page on the server that will receive the user data</li>
<li>method attribute: two options get or post. <ul>
<li>get: input data is added to the end of the action attribute URL<ul>
<li>best for short forms</li>
<li>when you are just retrieving data from the web server, not sending info that should be added/deleted to databases</li>
<li></li>
</ul></li>
<li>post: input data is sent in HTTP headers<ul>
<li>allows users to upload a form</li>
<li>best for long forms</li>
<li>if form contains sensitive data (passwords ect)</li>
<li>adds/deletes info in databases</li>
</ul></li>
</ul></li>
</ul>
