# Commenting Conventions

Commenting - not to be confused with [DocBlocks](docblock.md) - are used to make notes inside a section of code.

## Standard comment
Comments, regardless of the length, MUST use two forward slashes (`//`).
```php
// This is a comment
```

Comments can be spaced onto multiple lines.
```php
// This is a
// multi-line comment
```

Comments SHOULD NOT exceed the 80th column (80 character width).
```php
// This comment is so long that it will eventually reach the 80th column and will 
// need to be broken down into two lines.
```

The double asterisks (`/* */`) comment blocks signify a DocBlock, they SHOULD NOT be used.
```php
/*
This is an inappropriate comment type for inline documentation.
This is wrong.
*/
```

## NOTE Comment
Note/notice comments signify something more important than a normal comment.
```php
// NOTE: This is very important
```

## TODO Comment
TODO comments signify that something needs to be changed or improved with the code.
```php
// TODO: Implement better documentation
```
