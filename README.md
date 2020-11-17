Infinispan Embedded Migration
=============================

This project demonstrates how to perform a migration between applications using an embedded
Infinispan cache manager.


Usage
-----

Compile:

`$ mvn clean package`

Run the first instance (source):

`$ java -jar target/infinispan-playground-embedded-migration.jar -c src/main/resources/infinispan.xml`

Run the second instance (target):

`$ java -jar target/infinispan-playground-embedded-migration.jar -c src/main/resources/infinispan.xml -p 11223 -f hotrod://127.0.0.1:11222`

Once the migration is complete the source instance can be terminated with Ctrl-C.


