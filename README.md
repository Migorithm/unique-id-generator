## Globally unique identifier generator implementation in Rust
Generating globally unique identifier often takes importance especially when server-side ID generation is 
not appropriate choice for various reasons such as<br>
- when loads on backend storage is of your concern
- when using distributed system where you cannot access directly the id generating backend
- when mononotically increasing yet numerical values are required for ID

To solve the problems, Twitter took simple yet amazing approach using 64 bits data - `snowflake`. <br>
This project is Rust implementation of snowflake.