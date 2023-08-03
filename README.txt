Dropper

- Our dropper is implemented in the file dropper.py. 
- It tries to download some malicious code from a remote server and ideally avoid any detection. 
- The server is implemented in the file server.py and sends the malicious payload to the targeted system as soon as the dropper requests a connection. 
- Received payload is dumped into the file and the malware was successfully delivered.


Demonstration of behavior

- The first thing that the attacker must do is to set up a server that distributes malware to its clients. Therefore, set up a running server on our computer by running 
    - python3 ./server.py

- In the second console, execute the dropper as a victim with the command 
    - python3 ./dropper.py

- Our client has successfully connected to our server.

- To verify that the dropper has served its purpose, list the directory where the dropper is located and to see that a new file malware.py has been created. 
- For project demo purposes, the "malicious" code is just a simple command to print short text. 
