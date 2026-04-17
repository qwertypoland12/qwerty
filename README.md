# Php - wyświetlanie danych
## php connection
łączymy naszą bazę danych
```php
echo ("hello");
echo ('hello');
$connection = new mysqli("localhost","root","","test");
```

```php
$sql = "SELECT * FROM czlonkowie";
```

```php
$res = $connection -> query($sql);
```

```php
while($row = $res ->fetch_row()){
}
```



