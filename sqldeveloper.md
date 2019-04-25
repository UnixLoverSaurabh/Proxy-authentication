username: db20164104
password: db20164104

Hostname: 172.31.101.125
port: 1539
SID: orcl

./mysqlimport --local --host=172.31.100.41 -u 20164104 -p --fields-terminated-by=',' --fields-optionally-enclosed-by='"' --ignore-lines=1 db20164104 Q1_salesman.csv
