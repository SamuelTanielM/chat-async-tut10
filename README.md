# Chat Async Tutorial 10

Nama: Samuel Taniel Mulyadi

NPM : 2206081805


**Experiment 2.1: Original code, and how
it run**
> ![img.png](image/img.png)
> ![img_1.png](image/img_1.png)
> ![img_2.png](image/img_2.png)
> ![img_3.png](image/img_3.png)

In one of the exercises, I create a broadcast chat application using Rust. The server and client are implemented using WebSocket communication with the help of tokio_websockets crate.

To start, I'll need to set up a new Cargo project and add necessary dependencies in the Cargo.toml file. Then, I'll create two binaries: one for the server and one for the client. These binaries will be responsible for handling communication between the clients and the server.

In the server code (src/bin/server.rs), I implement the handle_connection function, which manages incoming client connections and broadcasting messages. In the client code (src/bin/client.rs), I'll handle sending user messages to the server and receiving messages from the server.

After completing the implementation, I can run the server and client binaries separately using cargo run --bin server and cargo run --bin client commands respectively.

After running the server and client, i set up two other clients in another two consoles separately. This program acts like a broadcast chat or a global chat, so if I send "hi" as client 1, the server and two other clients will see what i send, which is "hi", same as the two other clients, when they send messages, other can see it.

