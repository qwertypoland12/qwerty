# Php - wyświetlanie danych
## php connection
łączymy naszą bazę danych
```php
$connection = new mysqli("localhost","root","","test");
```
piszemy kod z sql
```php
$sql = "SELECT * FROM czlonkowie";
```

```php
$res = $connection -> query($sql);
```
wykonujemy pentle while
```php
while($row = $res ->fetch_row()){
}
```



