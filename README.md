# Bot-or-Not
Prediction of the Wikipedia data where the edit is made by Human or a Bot using Bigdata tools. Kafka, Spark, Postgre SQL

Wikipedia being the largest community of encyclopedia, most of the content is contributed by
human. But it also has bots which automate the content writing into Wikipedia. Wikipedia
publishes a stream of edits that are made to each of its articles and it provides a bunch of
different information in that stream it provides the name of the user, type of edit that was
made, how big it was made and the time when the edit was made. The aim is to predict
whether the edit is made by the human or a bot.

The Wikipedia data was fetched using hello-kafka- streams (A well-documented library to access the real-time edits data from Wikimedia API) developed in JAVA, obtained from developer community GitHub using IRC Wikimedia API. I had used Apache Spark in Python for connecting to Kafka topics to consume data every 2 seconds, process the data, store in Database and then apply Machine Learning on the received data. Python is a scripting language which has PySpark libraries and kafka streaming libraries for easier access to the nodes of Kafka. Postgre SQL, a relational database for persistent storage was used to create three tables for storage and fetching.

For further information regarding the project, please find the document "wikipedia".
