
<h1>HTML</h1>
  <p>-tags</p>
  <ul>
  <li>b: bold </li>
  <li>i: italics</li>
  <li>sup: superscript</li>
  <li>sub: subscript</li>
  <li>br: line break</li>
  <li>hr: horizontal line</li>
  <li>abbr title="": used for acronynms, uses a title attribute to provide the full name of the acronymn when moused over</li>
  <li>s: strikethrough text</li>
  <li>dfn: used for definitions or terminology</li>
  </ul>
  <p>css</p>
  <ul>
  <li>The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element</li>
  <li>Css rule syntax: 
    selector {property: value;}
    ex: h1, h2, h3 {color: blue;}</li>
  <li>link: used to link the html page to the css style sheet</li>
  <li>href: used as an attribute in the link tag to specify the location of the CSS file</li>
  <li>type: type of doc linked to</li>
  <li>rel: relationship to html page, should be 'stylesheet'</li>
  <li>ex: link href="css/style.css" type="text/css" rel="stylesheet"</li>
  <li>style: used instead of a seperate linked stylesheet, puts css on the html page</li>
  <li></li>
  </ul>
  <p>Selectors</p>
  <ul>
  <li>universal selector: *</li>
  <li>type selector: h1, h2, p etc</li>
  <li>class selector: . ex: .note</li>
  <li>id selector: #</li>
  </ul>
  <p>Cascading Rules</p>
  <ul>
  <li>The last rule: if two selectors are identical, the latter will take precedence</li>
  <li>Specificity: The more specific rule will take precedence</li>
  <li>Understanding this, you can right simpler Css sheets by writing general rules that apply to most elements and then write specific overriding rules for specific elements </li>
  </ul>
   