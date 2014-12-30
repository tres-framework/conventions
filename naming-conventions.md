Naming conventions
==================

*Scroll down for complete examples.*

## Namespaces
- Namespaces MUST make use of curly braces.
- Namespaces MUST use underscores where a space is expected.
- Namespaces MUST be lowercase unless it's a name, a country, a language, etc.
- Do not make a namespace to store exceptions.
- Every class, including abstract classes and interfaces MUST be inside a namespace.

The namespace path MUST match with the directory path. So let's take ExampleClass
as example. ExampleClass uses the "John_Doe\example_project" namespace.
In this case, the file should be John_Doe/example_project/ExampleClass.php

```php
<?php

// Wrong
namespace vendorName\packageName;
namespace John_Doe\db_search;

// Correct
namespace vendor_name\package_name {
    
    //
    
}

namespace John_Doe\db_search {
    
    //
    
}

```

## Classes
- Classnames MUST be written in PascalCase.
- Abbreviations MUST be written in FULLCAPS.
- Classnames MUST NOT contain underscores.
- Classnames names MUST contain alphanumeric characters.
- Classes SHOULD be given descriptive names.
- Only use abbreviations when very commonly used.

Numbers are permitted, but are discouraged in most cases.

```php
<?php

// Wrong
class user_model {
    
    //
    
}

class db {
    
    //
    
}

// Correct
class UserModel {
    
    //
    
}

class DB {
    
    //
    
}
```

## Abstract classes
Abstract classes follow the same convention as classes with one additional rule:
abstract classes SHOULD start with "Abstract" in their name.

## Interfaces
Interfaces follow the same convention as classes with one additional rule:
interfaces MUST end with "Interface" in their name.

## Filenames
Any file containing PHP code MUST end with .php.

## Functions and methods
- Function/method names MUST be written in camelCase.
- Abbreviations MUST be written in FULLCAPS.
- Function/method names MUST NOT contain underscores.
- Function/method names MUST contain alphanumeric characters.
- Function/method names SHOULD be given descriptive names.

Numbers are permitted, but are discouraged in most cases.

For methods on objects that are declared with the "private" or "protected" 
modifier, the first character of the method name must be an underscore. This is 
the only acceptable application of an underscore in a method name. Methods 
declared "public" should never contain an underscore.

```php
<?php

// Wrong
function HtmlPrettifier($html){
    //
}

class User {
    
    protected function getData(){
        //
    }
    
}

// Correct
function HTMLPrettifier($html){
    //
}

class User {
    
    protected function _getData(){
        //
    }
    
}
```

## Variables and properties
Variable/property names follow the same convention as functions/methods. 
Variable names like $i are only allowed in small loops.

```php
<?php

// Correct
class User {
    
    public $name = 'John Doe';
    
    protected $_status = 0;
    
}

```

## Constants
- Constants MUST contain alphanumeric characters and underscores.
- Constants MUST use underscores where a space is expected.

## Examples

```php
<?php

namespace John_Doe\account {
    
    class ExampleChild extends ExampleParent implements ExampleInterface, Example2Interface {
        
        public $exampleProperty = '';
        public $exampleProperty2 = 0;
        
        protected $_exampleProperty3 = [];
        
        private $_exampleProperty4 = '';
        
        const EXAMPLE_CONSTANT = 'value';
        
        public function __construct($exampleParam){
            $this->_exampleProperty3 = $exampleParam;
        }
        
        public function exampleMethod(){
            $data  = $this->_exampleMethod2();
            $data .= $this->_exampleProperty4;
            
            return $data;
        }
        
        protected function _exampleMethod2(){
            return $this->_exampleProperty3;
        }
        
    }
    
}

```
