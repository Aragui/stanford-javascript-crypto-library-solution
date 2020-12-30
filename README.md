# Use Stanford JavaScript Crypto Library Solution


###  The problem

In [this codepen](https://codepen.io/jlubean/pen/DHmtr) there is a implementation example for SJCL where you can play with the library, but it does nothing.

### The solution

The js script doesn't work because the script tag it's at the head tag of the document, when the interpreter reads the script the DOM doesn't exist yet.

Then the solution is, move this script tag to the bottom of the body and add JQuery.
