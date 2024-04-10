# Execute after redirect

```php
<?php
// In this page the page will be read and the content appended to the body of 
// the redirect response
$page = $_GET['page'];
header('Location: /index.php?page=default.html');
readfile($page);
?>
```
