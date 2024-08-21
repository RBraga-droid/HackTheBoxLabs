# Redeemer report

This simple excercise is used to familiarize with basic command of pentesting redis as a server tool. 

Following the commands in the chetsheet we use `redis-cli -h <host_ip> info` to display every information in the server, such as the version:

![image](https://github.com/user-attachments/assets/ed8f2091-9154-4666-b836-59686387e3f0)

And the keyspace of databases. We note a database by index 0 with 4 keys in it:

![image](https://github.com/user-attachments/assets/9194e39f-45d8-4313-9b6a-a269ef22a9e2)

We use the command `select 0` to eneter in the database and `keys *` to display every key. 

![image](https://github.com/user-attachments/assets/4b414f75-8b13-42a8-889b-bf476fcf6b54)

Then we can use `get <key>` to show the desired data, in this case we care about the flag:

![image](https://github.com/user-attachments/assets/3c5049ea-8ee9-45ac-870b-4b2ba7fe7070)
