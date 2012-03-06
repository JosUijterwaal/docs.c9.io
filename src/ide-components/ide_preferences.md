## IDE Preferences

There are many different ways to configure the IDE. Below is a list of these options:

Note: All of these options are on a per-project basis. Changing them in one project does not affect any another.

General
: This section controls the overall IDE behavior:

 * Enable UI Animations: enables or disables fluid animations for various UI elements, such as the Project Bar
 * Warn before exiting: Provides a dialog asking if you _really_ want to leave when closing your browser running Cloud9 IDE
 * Runtime: identifies the default runtime for your Node.js code. "Auto" is based on whatever is in the _package.json_ file, while "Default" reverts to Node 0.4.x.
 * On Save, Strip Whitespace: when saving a file, this will remove all extraneous whitespace from your code lines

Code Editor
: This section controls the IDE editor while you're coding:

* Auto pair Quotes, Brackets, etc.: when enabled, typing ", (,  or [ will actually make two characters appear. In addition, whenever you highlight a word and type one of these characters, it is surrounded by that character (e.g. words becomes "words")
* Code Folding: when enabled, allows you to show or hide "blocks" of code
* Full Line Selection: when highlighting lines, this option will highlight all ending whitespace, until the end of the editor window
* Highlight Active Line: presents a colored background to indicate which line you're currently on
* Show Invisible Characters: shows invisibles characters in the editor, like spaces, tabs, and line breaks
* Show Gutter: shows the gutter in the editor, which indicates line numbers, warnings, and errors
* Highlight Selected Word: when this is enabled, and if you highlight a word, this will highlight all matching words in the editor
* Auto-hide Horizontal Scroll: when this is enabled, this will hide the horizontal scroll bar in the editor. Note that this has no effect in Mac OS X 10.7 (Lion), since all scrollbars, by default, auto-hide.
* Font Size: changes the font size of the code in the editor
* Show print margin: shows (and defines) the number of characters possible in line, before it wraps
* Soft tabs: indicates how many spaces a single tab represents
* Mouse Scroll speed: defines the speed of the mouse scrolls
* Vim mode: when enabled, allows you to use vi keybindings

JS Beautify
: These options control the behavior of the code formatting tool found in **Edit | Beautify Selection**.  

* Preserve empty lines: if enabled, the editor keeps any new lines without text
* Keep array indention: when checked, tabs and newlines in arrays are preserved. For example, the follow array would remain as-is with this option:
    var o = [{
        a: b
    }, {
        c: d
    }];

* JSLint Strict Whitespace: if selected, all new scopes lines are indented by four spaces
* Braces: there are three options here:  
 * Braces with control statement: braces are left "in-line" alongside the code statements. For example, code is formatted like this:
    if (true) {
        var x = 3;
    } else {
        var x = 5;
    }

 * Braces on own line: braces are always placed on their own line. For example, code is formatted like this:
    if (true)
    {
        var x = 3;
    } else
    {
        var x = 5;
    }

 * End braces on own line: only the ending braces have their own line. For example, code is formatted like this:
    if (true) {
        var x = 3;
    }
    else {
        var x = 5;
    }

Language Support
: This section controls language analysis options:

 * Enable JSHint Rules: enables a layer of [JSHint warnings](http://www.jshint.com/) for your Javascript code
 * Highlight Instance Variables: highlights instance variables in your code
 * Mark Undeclared Cariables: provides warnings if a variable has not been declared yet
 * Mark Unused Function Arguments: creates a strikethrough for arguments in a function that are not being used