Database Design:
We will create a database named task_manager to store tasks. Each task will have the following attributes:
•	task_id: A unique identifier for the task (primary key)
•	title: The title of the task
•	description: A description of the task
•	status: The status of the task (e.g., "pending", "in progress", "completed")
•	due_date: The due date for the task
We will use a document-oriented database like MongoDB because it is well-suited for storing unstructured data like tasks. MongoDB stores data in JSON-like documents, which makes it easy to add, retrieve, update, and delete data.


Explanation of Database Organization:
We chose to use a document-oriented database like MongoDB because it is well-suited for storing unstructured data like tasks. MongoDB stores data in JSON-like documents, which makes it easy to add, retrieve, update, and delete data. Each task is stored as a separate document, and each document can have different fields. This makes it easy to add new fields to tasks without having to modify the schema of the database.
We also chose to use a primary key to identify each task. The primary key is the task_id field, and it is a unique identifier for each task. This makes it easy to retrieve, update, and delete tasks.
Finally, we chose to use indexes to improve the performance of queries. An index is a special data structure that allows you to query data more efficiently. We created an index on the due_date field to make it easy to query tasks by their due date.
