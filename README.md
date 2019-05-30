As a developer we should follow coding standards to make code homogeneous, easy to read and maintain.

### General Conventions
- The closing ``` ?> ``` tag must be omitted from files containing only PHP code
- Class file should not cross more than 350 lines & a method should not be more than 80 lines
- Break the line into multiple lines it is causing a horizontal scroll bar
- Try to break the logic into smaller functions, which can be reused later
- There **must not** be trailing whitespace at the end of lines
- All PHP files must end with one blank line
- ```try-catch``` should be used for the code causing exceptions
- There should not be empty ```Catch``` block, all exceptions **must** be handled.


### Naming Conventions
Variables **should** be declared using `camelCase` 
E.g:
```php
	$phoneNumber = 8098098089;
	$packageName = 'Test package';
```
Constants **must** be declared in all upper case with underscore separators 
E.g:
```php
	define('HOST_URL', 'http://localhost/test-project');
	
	// In class file
	const VERSION_NUMBER = '3.4.5';
	const STATUS = 'active';
```
Class names **must** be declared using `PascalCase` 
E.g:
```php
	class ProductDetails {
		// Do stuff here
	}
```
Method names **must** be declared using `camelCase` 
E.g:
```php
    /**
    * Returns product information
    */
	private function getProductDtls() {
		// Do stuff here
	}
``` 
Array names **should** be prefix with ```arr``` 
E.g:
```php
	$arrUserInfo = array(
		'name' => 'Sirisha',
		'phoneNumber => 8797973434,
		'email' => 'sirisha.grandhe@cognizant.com
	);
```
Object names **should** be prefix with ```obj``` 
E.g:
```php
	$objUser = new User();
```

### Class Conventions
* Always declare properties, methods with ```private``` scope & change them when needed
* Visibility must be defined for all properties & methods
* Property names should not be prefixed with ```Underscores```
* Methods must contain **comments** with the purpose of it in precise manner   
 E.g:
 ```php
    /**
    * Exports user information into in a CSV file
    */
    private function exportUserDtls() {
   		// Do stuff here 
    }
```
* Class name & the file name must be same
