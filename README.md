# ESRGclass

Start TCP Server
./server.elf port

Start TCP Client
./deamon.elf ip port

Client Send/Receive Messages
./client (msg)

Communication scheme

[Server] <---TCP----> [Deamon] <----MQUEUE-----> [Client]

Options
 - send messages server/client:	<"message">
 - close server/client connection: ctrl+c | "close"
 - every time a client send a message the server send the same message to all client
 - every 5 sec server checks the state client (message doesn't appear on chat)
 - if client didn't send a message in last minute changes his state from ONLINE to AFK
 - led on when client daemon is alive
 - led off when client daemon is dead
