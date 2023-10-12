# Data Science Extensions

Fork of original data science extensions library, with some specific alterations.

# Building from source

First install maven and java:

```
apt-get install openjdk-11-jre-headless
apt-get install maven
```

## For debugging

mvn -Drat.ignoreErrors=true package

## Release

```
mvn clean install -pl spark-datasource-rest -DskipTests -Dscalastyle.skip=true
```

# Use in spark-shell

run: `spark-shell --jars "spark-datasource-rest/target/spark-datasource-rest_2.12-3.3.1-SNAPSHOT.jar"`

In the scala session, run:

``` 
import org.apache.dsext.spark.datasource.rest._
```

You can now use all the different classes and objects in the library.