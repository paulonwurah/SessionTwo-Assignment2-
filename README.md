Assignment Two 

1. The relation between workers, executors and task goes thus; workers are the slaves in the spark cluster that encapsulates processing of partitions of RDD (Resilient Distributed Dataset). In actual sense, workers are not what does the processing and computation but executors which are assigned by the cluster manager to the workers when 'Spark Context' connects to the cluster manger. Executors are spaces in a worker that does the actual processing and computation. A worker can have more than one executor performing many processing and computation on partitions of different RDDs (Resilient Distributed Data-set). To perform the processing and computation on the partitions in the executors, tasks are needed.  A task is a command sent from the driver to an executor by serializing your Function object. The executor deserializes the command and executes it on a partition.

2. The key feature of spark includes:

 A. Lighting Fast Processing: In big data processing, speed and time always matter. There is always a need for processing very huge data as fast as possible. Spark enables application in Hadoop cluster to run about 100x faster due to its memory computation (RAM) and 10x faster even when running on disk. This is possible because spark reduces the number of read and writes that is done on a disk. Its intermediate processing data is stored in memory. There is a concept know as Resilient Distributed Dataset (RDD) spark uses which allows it to store data on memory and only persist to disc only when its needful to. This process helps reduce most of the disc read and write which is the main time consuming factor of data processing.

 B. Richly Diversified API's: Spark lets you write applications in different languages such as Java, Scala and Python. This gives developers comfort as they are able to create and run their applications on their familiar programming languages

 C. Supports Sophisticated Analysis: In addition to the basic 'map' and 'reduce' operations, spark supports SQL queries, streaming data and other complex analytics such as machine learning and graph algorithm out of the box. The beautiful thing about spark is that a user can combine all these capabilities seamlessly in a single workflow. 

 D. Handling of Real Time Processing: Spark is able to handle real time streaming. Map-reduce can mainly just handle and process the data stored already while Spark can manipulate both data stored over time (batch) as well as data in real time, the latter is done using spark streaming. There are other frameworks with their integration we can handle streaming in Hadoop but why would you need to learn different frameworks to get what you can do with just learning one framework which is widely agreed upon by various vendors that it is easy, fault tolerant and integrated. 

 E. Ability to Integrate with Hadoop and Existing Hadoop Data: Spark can run independently but they made it in such a way that you can migrate easily from Hadoop to spark or even use some Hadoop features with spark such as its data, distributed database (HBase) and its distributed file system (HDFS). That’s a very BIG advantage as companies already using Hadoop application can migrate to spark if the application is really suiting spark.  Not all scenarios might be suitable for spark as spark uses immutability more.

 F. Active and Expanding Community: Apache is built by a wide set of developers from over 50 companies. The project started in 2009 and as of now, there are more than 250 developers that have contributed to spark already. It has active mailing lists for tracking purposes.

3. Spark driver is the program that runs on the master node of the machine and declares transformations and actions on data RDDs. The driver also delivers RDD graph to the master where the cluster manager runs.

4. The benefits of spark over map reduce are:
 A. Spark is easier to program and does not require any abstraction.
 
 B. Spark has an interactive mode 
 
 C. Spark makes it possible to perform streaming, batch processing and machine learning all in the same cluster
 
 D. Spark has been said to execute batch processing jobs near about 10 to 100 times faster than Hadoop 
 
 E.  Spark can be used to modify the data in real time through spark streaming
 
 F. Spark ensures lower latency computation by caching the partial results across its memory of distribution
 
 G. Writing Spark code is always compact than writing Hadoop Map Reduce code.

5. When 'Spark Context' connects to a cluster manager, it acquires an 'Executor' on the cluster nodes.  ‘Executors' are Spark processes that run computations and store the data on the worker node. The final tasks by 'Spark Context' are transferred to executors.
6. 30 mins 
