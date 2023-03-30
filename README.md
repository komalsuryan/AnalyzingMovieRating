# AnalyzingMovieRating
You are required to analyze a movie rating dataset. The data is stored in a CSV file (either use the one in the repository or download the latest from Kaggle). You need to read this file into spark and calculate the mean rating and standard deviation for all movies. There is no test case provided for you, so you need to write your own test cases to ensure that at least your program works well.

You can refer to WordCount.scala file for the basic structure. Notice that you need to use specific Spark version 3.2.1 for Scala 2.12.x support. If you can run it using a version with Scala 2.13, then go ahead.

Note also that there is a module in the CSYE7200 repository called spark-csv. If you use that, you will have to edit the build.sbt file. You can use that code of course to get started with (show your results if you do this). However, you also need to read the CSV file using the Spark utility (see https://spark.apache.org/docs/3.2.1/sql-data-sources-csv.html) and then create a method that accepts a DataFrame and returns the processed DataFrame.

You need to provide your code (in your own repository) together with the mean/std. dev. Don't forget to say where exactly you got the CSV file from.

Unit Tests:

Test case 1: When the column name is valid and contains numerical values, the method should return the correct average of the column.

Test case 2: When the column name is valid but contains non-numerical values, the method should return null.

Test case 3: When the column name is valid and contains numerical values, the method should return the correct standard deviation of the column.
