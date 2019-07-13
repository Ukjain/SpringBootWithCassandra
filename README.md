# SpringBootWithCassandra

Install Cassandra

Install Cassandra
  sudo apt-get install cassandra
	sudo service cassandra setup / Check if it is running

Setting up keyspace and sample schema
	 keyspace
  	Create keyspace “employee” with replication = { ‘class’: ‘SimpleStrategy’,’replication_factor’ : ‘1’};
	  use employee
	  Create table employee_profile (id BigInt Primary Key, name text, age int, salary float);
	  insert into employee_profile(id,name,age,salary) values (1,’Max’,29,10000);
	  select * from employee
