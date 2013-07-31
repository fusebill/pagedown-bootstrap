PageDown-Bootstrap
==================

This is a fork of http://code.google.com/p/pagedown/ changed to use Twitter Bootstrap for styling the editor and modal popups.

The demo is viewable here: http://samwillis.co.uk/pagedown-bootstrap/demo/browser/demo.html

New icons based on http://glyphicons.com/, http://dribbble.com/shots/365544-Mini-glyphs-12-px-Free-PSD and the origional icons.

* There were three key issues that were solved locally which is why this package is not being included from the Nuget package source:

 - The menu buttons were acting like submit buttons when pressing Enter.  Changed button types to type button.
 - Dialog boxes were submitting the main form when pressing Enter.  There were two issues to be solved:
   - The buttons were not of type submit
   - The buttons were not inside the form.  We ordered how elements were appended to wrap the modal-body and modal-footer inside the form.