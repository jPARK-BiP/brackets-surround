# Surround for Brackets - pedelman

Simply select the text you wish to surround and press ```Ctrl - Shift - J``` or ``` Cmd - Shift - J``` for Macs.

#### Installation

Installation can now be handled through the extension registry.

##### Step 1: Click file -> "Extension Manager"

You can now search for "Brackets Surround" and then click install.

---

#### For Older Versions
##### Step 1: Click file -> "Install Extension"

Paste in the following URL

```
https://github.com/jPARK-BiP/brackets-surround
```

##### Step 2: Restart brackets
Restart Brackets to see the new plugin. To verify the extension was loaded, click "Edit" and you should see a option called "Surround".

---

#### Easy to add new functionality

```js
cases = {
   '('    :   ')',
   '{'    :   '}',
   '<'    :   '>',
   '['    :   ']',
   '/*'   :  '*/',
   '<!--' : '-->',
   '<%'   :  '%>',
   '<%='  :  '%>'
};
```

Simply add a new key/value to the cases and it will instantly close the key.

---

#### Bugfixes - jPARK-BiP

Sometimes when input ends in punctuation (if you accidentally hit enter after a '.' rather than '>' for example) Brackets can crash completely, thus losing whatever document you were working on and carelessly not saving every few seconds (not that I ever did that).

This update checks for the last character in the input string and exits the surround box if it ends in:

, - comma
. - full stop
; - semi-colon
' - inverted comma
/ - fwd slash

(closest to '>')

This may not be useful for some people, if you actually need to end the string in those characters for example, but since it crashes every time I put them in, I'm guessing it may be the same for a lot of people.