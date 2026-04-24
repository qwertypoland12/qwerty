# Php - wyświetlanie danych
## php connection
łączymy naszą bazę danych
```php
$connection = new mysqli("localhost","root","","test");
```
piszemy kod z sql
```php
$sql = "select imie, Nazwisko from czlonkowie INNER join karnety on czlonkowie.id_czlonka = karnety.id_karnety;";
```

```php
$res = $connection -> query($sql);
```
robimy pętle While, (fetch_row)
```php
while($row = $res ->fetch_row()){
}
```
zapisujemy znaczenie do tabeli dla id
```php
echo 
    "
        <tr>
            <td>{$row[1]}</td>
            <td>{$row[2]}</td>
        </tr>
    ";

```



