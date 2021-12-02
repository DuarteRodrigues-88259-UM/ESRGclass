# ESRGclass

# Start Server
./tcpserver.elf port

# Star Client
./tcpclient.elf ip port (str)

# Options
 - send messages server/client:	<"message">
 - close server/client connection: ctrl+c | "close"
 - every time a client send a message the server send the same message to all client
 - every 5 sec server checks the state client (message doesn't appear on chat)
 - if client didn't send a message in last minute changes his state from ONLINE to AFK
