Tres conventions
================

When contributing to Tres, you must follow the conventions.

Well documented and followed conventions results in readable and unambiguous 
source code. That is exactly what we are trying to achieve.

To keep a codebase consistent, you should always follow one convention. Because 
you standardize the structure and coding style, others can easily read and 
understand the code.

## EditorConfig

EditorConfig helps developers define and maintain consistent coding styles 
between different editors and IDEs. The EditorConfig project consists of a 
file format for defining coding styles and a collection of text editor plugins 
that enable editors to read the file format and adhere to defined styles. 
EditorConfig files are easily readable and they work nicely with version 
control systems.

Tres follows the following EditorConfig.
```
root = true

[*]
charset = utf-8
indent_style = space
indent_size = 4
trim_trailing_whitespace = false
insert_final_newline = true

```
Please, make use of it when possible.

*Read more at [editorconfig.org](http://editorconfig.org/).*
