DocBlock Conventions
=====================

DocBlocks are an efficient way of explain a section of code. DockBlocks helps to explain the parameters a function/method takes and the expected outputs.

Skip to a section
* [Classes](#classes)
* [Functions/Methods](#functionsmethods)

## Classes
Tres Framework **highly** discourages the use of DocBlocks for classes whenever possible, instead use [package.json](conventions/package.json.md). Using package.json allows interfacing with other Tres packages and better detail about the the packages limitations/requirements. If you need/wish to use a DocBlock follow the following format.

### Format
* Use only asterisks, pipes & dashes.
* Dashes should not exceed the 80th column (80 character)
* Content should wrap to the next line at the 80th column (80 character)
* Use the appropriate `@param <info>`, ex.
```
@version  0.0.0
@author   Last, First <author@email.tld>
@author   Last, First <author@email.tld>
@link     git link
@License: The MIT License (MIT)
```


### Examples
#### Asterisk
```php
/**
 *------------------------------------------------------------------------------
 * ClassName - optional short desc.
 *------------------------------------------------------------------------------
 * 
 * Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
 * tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 * quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 * consequat.
 * 
 */
```
#### Pipes
```php
/*
|-------------------------------------------------------------------------------
| ClassName - optional short desc.
|-------------------------------------------------------------------------------
| 
| Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
| tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
| quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
| consequat.
| 
*/
```
#### Kitchen Sink
```php
<?php
namespace vendor_name\project_name {
    /**
     *--------------------------------------------------------------------------
     * KitchenSink - Every and the kitchen sink
     *--------------------------------------------------------------------------
     * 
     * The Kitchen Sink allows all the features plus more. Take your sink to the 
     * next level with the Kitchen Sink. The Kitch Sink has all the features one 
     * would expect of a kitchen sink. It's a sink in the kitchen which does 
     * things a kitchen sink would do like rinsing, cleaning, soaking. The 
     * Kitchen Sink has so many features.
     * 
     * @version  1.2.0
     * @author   Doe, John <john@doe.tld>
     * @author   Doe, Jane <jane@doe.tld>
     * @repo     https://github.com/organization/forceDownload
     * @License: The MIT License (MIT)
     */
    class KitchSink {

        // ...

    }

}
```

## Functions/Methods
### Format
* Use only asterisks, pipes & dashes.
* Dashes should not exceed the 80th column (80 character)
* Content should wrap to the next line at the 80th column (80 character)
* Only use the `@param` & `@return`

### Data types
| Type       | Alternative | Note |
|------------|-------------|------|
| `integer`  | `int`       |      |
| `string`   | `str`       |      |
| `array`    |             |      |
| `object`   | `obj`       |      |
| `null`     |             |      |
| `boolean`  | `bool`      |      |
| `float`    |             |      |
| `callback` |             |      |
| `variadic` | `$...`      |      |
| `mixed`    |             | While using mixed is acceptable it is recommended to list the appropriate data types with a a pipe ( &#124; ). Example: array&#124;str&#124;object. |

### Basic
```php
/**
 * Short description for file
 *
 * Long description for file (if any)...
 *
 * @param  string $variable  Short description...
 * @param  int    $variable2 Short description...
 * @return object            Short description...
 */
```

### Multiple data types
When listing a variable with multiple possible data types you can use a pipe (`|`).
```php
/**
 * Short description for file
 *
 * Long description for file (if any)...
 *
 * @param  string|array $variable  Short description...
 * @param  int          $variable2 Short description...
 * @return object                  Short description...
 */
```
You can also list them on multiple rows.
```php
/**
 * Short description for file
 *
 * Long description for file (if any)...
 *
 * @param  string $variable  Short description...
 * @param  array  $variable  Short description...
 * @param  int    $variable2 Short description...
 * @return object            Short description...
 */
```







































