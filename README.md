# ESRGclass

Execute Makefile

Make all        Compile and generate the object files

Make clean      Delete the object files

Make transfer   Copy the file to raspeberry

Notes:
    CC_r        Raspberry Compiler 
    
    CC_h        Host Compiler
    
    IP          Raspberry IP


Start TCP Server
./server.elf port               (Host/Target)

Start TCP Client
./deamon.elf ip port            (Host)
./daemon_rasp.elf ip port       (Target)

Client Send/Receive Messages    (Host/Target)
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

# Done by
João Miranda 88237

Duarte Rodrigues 88259

Masters in Embedded Systems @ Universidade do Minho, 2021
