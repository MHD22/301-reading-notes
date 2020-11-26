##### [back-home](https://mhd22.github.io/301-reading-notes/)


# Read: 11 - EJS

## What is EJS?


What is the "E" for? "Embedded?" Could be.

How about "Effective," "Elegant," or just "Easy"? EJS is a simple templating language that lets you generate HTML markup with plain JavaScript. 

No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript.

#### _____________________________________________

**It's easy to install EJS with NPM.**

`$ npm install ejs`

#### _____________________________________________

### Use
**Pass EJS a template string and some data. BOOM, you've got some HTML.**

```let ejs = require('ejs');
let people = ['geddy', 'neil', 'alex'];
let html = ejs.render('<%= people.join(", "); %>', {people: people});

```
#### _____________________________________________

## Tags:

`<%` 'Scriptlet' tag, for control-flow, no output

`<%_` ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it

`<%=` Outputs the value into the template (HTML escaped)

`<%-` Outputs the unescaped value into the template

`<%#` Comment tag, no execution, no output

`<%%` Outputs a literal '<%'

`%>` Plain ending tag

`-%>` Trim-mode ('newline slurp') tag, trims following newline

`_%>` ‘Whitespace Slurping’ ending tag, removes all whitespace after it


#### _____________________________________________

## Custom delimiters

***Custom delimiters can be applied on a per-template basis, or globally:***

```
let ejs = require('ejs'),
    users = ['geddy', 'neil', 'alex'];

// Just one template
ejs.render('<?= users.join(" | "); ?>', {users: users},
    {delimiter: '?'});
// => 'geddy | neil | alex'

// Or globally
ejs.delimiter = '$';
ejs.render('<$= users.join(" | "); $>', {users: users});
// => 'geddy | neil | alex'

```












#### _____________________________________________



### This file wrote by [Mohamad Saad Eddin](https://github.com/MHD22).
***you can visit my profile and follow me.***
### ______________________________________________


###### Thanks for your time, I hope that you have enjoyed.