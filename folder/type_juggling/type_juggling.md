# Loose comparisons with ==

<https://www.php.net/manual/en/types.comparisons.php>
![comparision table](image.jpg)

- TRUE: "0000" == int(0)
- TRUE: "0e12" == int(0)
- TRUE: "1abc" == int(1)
- TRUE: "0abc" == int(0)
- TRUE: "abc" == int(0) // !!
- TRUE: "0e12345" == "0e54321"
- TRUE: "0e12345" <= "1"
- TRUE: "0e12345" == "0"
- TRUE: "0xF" == "15"
===
### example
```php
if (Session::token() != Input::get('_token'))
{
throw new Illuminate\Session\TokenMismatchException;
}
```
| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |
