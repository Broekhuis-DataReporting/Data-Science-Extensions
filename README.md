# Data Science Extensions

Fork of original data science extensions library, with some specific alterations.

# Installation

mvn -Drat.ignoreErrors=true package

# Use in spark-shell

run: `spark-shell`

In the scala session, run:

```
:require spark-datasource-rest/target/spark-datasource-rest_2.12-3.3.1-SNAPSHOT.jar
import org.apache.dsext.spark.datasource.rest._
```

You can now use all the different classes and objects in the library.