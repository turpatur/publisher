1. How much data your publisher program will send to the message broker in one
run?
- Publisher akan mengirimkan 5 data karena mengirimkan 5 publish_event.
- Untuk setiap publish event ada user_id dengan 1 karakter -> 1 byte
- Ada juga user_name dengan 15 karakter -> 15 byte 
- Maka total adalah (15 + 1) * 5 = 80 byte

2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber
program, what does it mean?
- Ya, sama. Artinya, publisher dan subscriber akan terhubung pada server amqp yang sama dengan credentials, host, dan port yang sama. 