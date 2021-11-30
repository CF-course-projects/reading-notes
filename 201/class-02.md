-html
  -tags
    <b>: bold 
    <i>: italics
    <sup>: superscript
    <sub>: subscript
    <br />: line break
    <hr />: horizontal line 
    <abbr title="">: used for acronynms, uses a title attribute to provide the full name of the acronymn when moused over 
    <s>: strikethrough text
    <dfn>: used for definitions or terminology
-css
  The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element
  Css rule syntax: 
    selector {property: value;}
    ex: h1, h2, h3 {color: blue;}
    <link/>: used to link the html page to the css style sheet
    <href>: used as an attribute in the link tag to specify the location of the CSS file
    <type>: type of doc linked to
    <rel>: relationship to html page, should be 'stylesheet'
    ex: <link href="css/style.css" type="text/css" rel="stylesheet"/>
    <style>: used instead of a seperate linked stylesheet, puts css on the html page
  -selectors
    -universal selector: *
    -type selector: h1, h2, p etc
    -class selector: . ex: .note
    -id selector: # 
  Cascading rules:
    -The last rule: if two selectors are identical, the latter will take precedence
    -Specificity: The more specific rule will take precedence
    Understanding this, you can right simpler Css sheets by writing general rules that apply to most elements and then write specific overriding rules for specific elements 
