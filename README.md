# PHP Functions

Display PHP errors

```php
ini_set('display_errors', 1);
ini_set('display_startup_errors', 1);
error_reporting(E_ALL);
```

Capitalize first letter

```php
ucfirst('hello world');

// hello world -> Hello world
```

Capitalize all words

```php
ucwords('hello world');

// hello world -> Hello World
```

Replace values in string

```php
str_replace('-', ' ', 'hello-world');

// hello-world -> hello world
```

Find index of first value in a string

```php
strpos('hello world', 'hello');

// 0
```

Make a string lowercase

```php
strtolower('HELLO world');

// HELLO world -> hello world
```

Make a string uppercase

```php
strtoupper('HELLO world');

// HELLO world -> HELLO WORLD
```

Comma separate values in an array

```php
$arr = [1, 2, 3];

foreach ($arr as $value) {
    $comma_separated = (!empty($comma_separated)) 
    ? $comma_separated .= ', ' . $value 
    : $comma_separated = $value; 
}

// $comma_separated -> "1, 2, 3" (string)
```

Create an array from a string

```php
$arr = 'one two three';
$each = explode(' ', $arr);

// $each[0] -> 'one'
```

Push to an array

```php
foreach ($arr as $value) {
  $newArray[] = [
    'id'   => $value['id'],
    'name' => $value['name'],
  ];
}
```
