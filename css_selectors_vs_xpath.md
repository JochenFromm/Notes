
# CSS selectors vs XPATH

[XPath and CSS Selectors](https://johnresig.com/blog/xpath-css-selectors/)
are commonly used to find elements in a web page.

XPath stands for XML Path and is a query language to identify elements 
from an XML document - or an web page in HTML. It is common for Selenium.

CSS selectors define a pattern to select elements in a HTML page too.
The syntax is similar, but slighty different.


|                         | CSS Selector            | XPATH                               |
| ----------------------- | ----------------------- | ----------------------------------- |
| All elements            | *                       | //*                                 |
| All p elements          | p                       | /p                                  |
| Element by ID           | #root                   | //*[@id='root']                     |
| p element by ID         | p#paragraph             | //p[@id='paragraph']                |
| Element by class        | .name                   | //*[@class='name']                  |
|                         |                         | //*[contains(@class,"name")]        |
| Element by two classes  | .name1.name2            | //*[@class='name1 name2']           |
| p element by class      | p.name                  | //p[contains(@class,"name")]        |
| p element by attribute  | p[attr="value"]         | //p[@attr="value"]                  |
| Direct child            | head > title            | //head/title                        |
| Child                   | html title              | //html//title                       |
| element containing text | - not possible -        | //p[contains(text(), 'Hi there')]   |
| 2nd row in table        | table tr:nth-of-type(2) | //table//tr[2]                      |
