# Spark 
### Task 1 (Notebook 1)
Our goal is to create a predictive model that can answer the following question:

What kind of people had a better chance of surviving?


### Task2 (Notebook2)
- Create streaming DataFrame
Let’s create our first Spark Streaming DataFrame using "rate" format. Here we have specified the format as rate and specified rowsPerSecond = 1 to generate 1 row for each micro-batch and load the data into initDF streaming DataFrame.
- Transformation: Word Count
Here we count words from a stream of data coming from this socket. Also, we check the schema of our streaming DataFrame.

### Task 3
Some aggregations transformation
Select "Name","Date", "Open", "High", "Low" and group by Name and Date and get the avg and use WithColumn to get current_timestamp

### Task 4
One-time micro-batch
With a once trigger, our query will execute a single micro-batch. It will process all available data and then stop the application. This trigger is useful when you would like to spin-up a cluster periodically, Execute our streaming application with the once trigger.

### Task 5 
Users can create GraphFrames from vertex and edge DataFrames.
Vertex DataFrame: A vertex DataFrame should contain a special column named “id” which specifies unique IDs for each vertex in the graph.
Edge DataFrame: An edge DataFrame should contain two special columns: “src” (source vertex ID of edge) and “dst” (destination vertex ID of edge).

- Create UDF Functions
convert your graph by mapping a function over the edges DataFrame that deletes the row if src ≥ dst return "Delete" else "Keep"

- Filtering and connected components

