#coursera- HTML, CSS, Java script

HTML


Module 1: Basic HTMl structure
  1) always start with <! doctype HTML> - tells the compiler the document should be interpreted in HTML languate
  2) <html> - <meta> - <head> - <title> - <body> - Typical sequence of a HTML document
  3) Bloc level elements (e.g. <div>) - Renders in a new line and pushes the following elements to a new line; can contain      both inline and bloc level elements; if the child element is an inline element, then the child is rendered on the same      line
  4) Inline (e.g. <span>)- Renders on the same line; can contain only inline elements
  
  
Module 2: Tags

  Signifiance of tags:
    1) Give structure and readability to code
    2) May help in SEO search rankings
    
  Head tags:
    1) <h1> -> Most importanat headings, defenitely helps in SEO rankings
    2) <h2>
    3) <h3>
    4) <h4>
    5) <h5>
    6) <h6> -> Least important heading of the document
    
Header and navigation tag:
  1) <header> - Logos, tag lines and as such
  2) <nav> - Contains links to different parts of the web page
  
Section and article tag:
  1) <section>
  2) <article>
      Both tags can be used interchangably. But for code readbility, article tags are placed in side section tags always
      
 Aside tag:
  <aside> - related but not part of the main contect
 
 Footer tag
  <footer> - Contains the footer
  

Module 3: Lists
  
   Unordered lists:
    1) <ul> 
          <li> Item 1 </li>
          <li> Item 2 </li>
          <li> Item 3 </li>
       </ul>
       - Bulleted list by default
       - All elements inside <ul> tags must be a <li> item
       - We can edit the bullet style through CSS
       
   Ordered lists:
    1) <ol> 
          <li> Item 1 </li>
          <li> Item 2 </li>
          <li> Item 3 </li>
       </o>
       - Numbered list by default
       - All elements inside <ul> tags must be a <li> item
       - We can edit the bullet style through CSS

    
Module 4: Character entity referencing

  Used to differentiated HTML elements and contents
  Most commonly used character entity referencing:
    1) &lt; -> will be interpreted as <
    2) &gt; -> will be interpreted as >
    3) &amp; -> will be interpreted as &
    4) &copy; -> will be interpreted as the copyright symbol
    5) &nbsp; -> will be interpreted as a non breaking space
              -> Caution: Dont use the &nbsp; tag to creat extra space. It is a bad practice. Use span tag with margins
    6) &quot; -> will be interpreted as double quotes
              -> All charater inside the entity reference will be rendered as it irrespective of the browser character set
    
    
Module 5: Creating links

  There are two type of links: 1) Internal link (Links internal to the HTML document) 2) External link (Links that point to   other web pages and documents 3) Fragment identifier (Links to different parts of the same web page)
  
    1) Internal links:
      <a href="same-directory.html" title="same dir link"> 
        -> attributes: 
            href: Link address 
            title: title of the link; used for code readability
        -> <a> is both inline element and bloc level element
        
    2) External links:
      <a href="https://github.com/ravindra-sagar/coursera-test/edit/main/README.md" target="_blank" title="external link">
        -> attributes:
          href: Link address
          target: "_blank" forces the browser to open the link in a new tab
          title" title of link; used for code readability
    
    3) Fragement identifier:
        <a href="#section_name_or_id">
          -> attributes:
              href: must have # followed by name or id of the HTML element it is refering to
    
          
  Module 6: Display images
          
    <img src="Link.jpg" width="400px" height="235pg" alt ="Pics">
          -> Functions very similar to link, it is an inline element, hence other element
          -> Attributes:
              src: Link to the image (can be internal or external)
              width: Prevents the web page from being jumpy
              height: Prevents the web page from being jumpy
              alt: Specified alternate text if image could not be loaded
          
          
 
CSS:

  Module 1: General CSS rules
    1) Always create a seperate CSS stylesheet with ".css" doctype and link it in the main HTML file
    2) Must be enclosed by <style> tag
    3) General anatomy:
          element {
            attribute1: value1;
            attrribute2: value2;
            .
            .
            .
          }
          
  Module 2: CSS selectors
    1) Indicates which elements, class or ID, the CSS style should be applied to
        a) Element selector:
            p {
              width: 100px;
              height: 50px;
            }
        b) Class selector:
            .class_name {
              width: 100px;
              height: 50px;
            } 
              -> Must always be defined as . followed by class name
              -> To use the style, the element should be formatted as: <p class="class_name">
        c) ID selector:
            #ID {
              width: 100px;
              height: 50px;
            } 
              -> Must always be defined as # followed by ID name
              -> To use the style, the element should be formatted as: <p ID="class_name">
  2) Grouping selectors
      selector1, selector 2 {
            attribute1: value1;
            attrribute2: value2;
            .
            .
            .
          } 

  Module 3: Combining selectors
    1) Element and class combination
          selector_name.class_name {
            attribute1: value1;
            attrribute2: value2;
            .
            .
            .
          }
        -> Style applied only to content of selector_name and class as class_name
          
    2) Direct child selector
          selector1 > selector2 {
            attribute1: value1;
            attrribute2: value2;
            .
            .
            .
          }
          -> Style applied only to content of selector2 which are direct children of selector1

    3) Descendant selector
          selector1 selector2 {
            attribute1: value1;
            attrribute2: value2;
            .
            .
            .
          }
          -> Style applied only to content of selector2 which are descendeants (direct or indirect children) of selector1

    4) Other selectors:
          a) Adjacent selector
          b) Sibling selector
          
 
