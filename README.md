# cv-worker overall idea
Just started ...
The idea is to create a parent worker service that spawn child workers to execute opencv tasks like image matching, OCR ...
* Tasks are added into a RabbitMQ queue and consumed by available child workers.
* A task is typically a json object that describes the details of an operation to perform: commande line & parameters.
