File formatting
===============

## General
Files ending with PHP code may not have the closing PHP tag. Ommiting it 
prevents accidental white space which may result in the common 
"Headers already sent" error.

## Indentation
Use an indent of 4 spaces with no tabs.

## Line length
Soft limit: 80
Hard limit: 120

Try to keep your line length within the soft limit. You may not exceed the 
hard limit.

Tip: some text editors like Sublime Text have to option to show rulers
(vertical lines), so you can easily see where your limit is.

For Sublime Text, add the following code in the user settings:
```
"rulers": [80, 120]
```

## Line termination
Lines must end with a single linefeed (LF).

Tip: EditorConfig gives you the option to do this automatically.
