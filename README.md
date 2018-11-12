# CC-proj
Distributed architecture implementation on Amazon AWS

Challenges

Application should run locally on your machine

User inputs a comma-separated list of numbers.

Puts this list in the S3-bucket (and remembers the key/pointer to this object).

Puts a message in the SQS-inbox with a key/pointer to the object in the S3-bucket, along with a process to be executed on these numbers.

Waits until a response is generated in the SQS-outbox (should contain a pointer to a new, and processed, object in the S3-bucket along with the process executed).

Reads the result from the S3-bucket

Prints the results along with the original numbers and the the process that was done.

Deletes the result-message from the SQS-outbox.
