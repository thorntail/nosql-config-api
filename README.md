Generate Thorntail NoSQL fractions Configuration API.
Supports generating fraction Config API for NoSQL subsystems in https://github.com/wildfly/wildfly-nosql

Steps to generate `nosql-config-api`:

1.  git clone https://github.com/wildfly/wildfly-nosql
2.  cd wildfly-nosql
3.  mvn clean install
4.  cd server/target/wildfly-nosql-serverbuild/bin
5.  ./standalone.sh
6.  open additional terminal shell and continue in the `nosql-config-api` directory
7.  cd nosql-config-api
8.  mvn clean install
9.  done, verify with `find -name *.java`, you should see `./mongodb/target/generated-sources/org/wildfly/swarm/config/mongodb/Mongo.java` and other files as well.
10. if you don't see any generated files, something is wrong.
11. stop the app server started in step #5

See https://github.com/thorntail/wildfly-config-api/blob/master/README.md for instructions from the master project that `nosql-config-api` is cloned from.
