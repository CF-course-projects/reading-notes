### Debugging
<p>Error Objects</p>
<ul> Error objects have 4 properties:
<li>Type of error</li>
<li>Description</li>
<li>Name of the JavaScript file</li>
<li>Line number of error</li>
</ul>
<p>Types of Error Objects</p>
<ul> 7 types of Error objectss:
<li>Error: Generic error - all other errors are based on this</li>
<li>SyntaxError: syntax has not been followed</li>
<li>ReferenceError: Tried to reference a var that is not delcared/within scope</li>
<li>TypeError: An unexpected data type that cannot be coerced</li>
<li>RangeError: Numbers not in acceptable range</li>
<li>URIError: encodeURI(), decodneURI(), and similiar methods used incorrectly</li>
<li>eval() functon used incorrectly</li>
</ul>
<p>Debugging workflow</p>
<ul>
<li>Analyze the error message: they are your friend</li>
<li>describe what your code is doing to another programmer: can be imaginary</li>
<li>use console.logs to see how far your script is running before breaking</li>
<li>check what functions are returning</li>
<li>check if objects exists/can be accessed</li>
<li>check contents of arrays etc.</li>
</ul>
<p>Breakpoints: You can pause the execution of a script on any line using breakpoints</p>
<ul>
<li>Select the Sources option</li>
<li>Select the script you are working with</li>
<li>Find the line number you want to stop on and click on it</li>
<li>When you run the script, it will stop at this breakpoint</li>
<li>Conditional Breakpoints: <ul>
<li>right click on a line number</li>
<li>select add conditional breakpoint</li>
<li>enter a condition into the popup box</li>
</ul></li>
</ul>
<p>Throwing errors to avoid more problematic errors: You can use the method isNaN() with throw new Error() for example to throw an error before calculating further</p>



