================================================================

    README file for Assignment 1 - HTTP Proxy

           Name: 
 Username/Login: 
 
================================================================

## Steps to run the assignment:
### Step 1: Inputting the HTTP request:
- In the file **request_generator.c**,enter the request within the **printf** statement in main, followed by "\r\n\r\n" for CLRF characters.
- This was not mentioned earlier,because we assumed that the mechanism to generate an HTTP request was already present with the evaluator.
- This step can be skipped if another mechanism to generate a well-formatted request exists. This is only our suggested way of doing so, as we had difficulties with entering CRLF in terminal.
### Step 2: Building the configuration
`$>` `make` 
(This generates two executables: **proxy** and **request**.)
### Step 3: Running the program
- `$>` `./request >telnet_input.txt` (This writes the formatted input to a file. This is done, because it is not possible to enter CRLF in a terminal window to the best of our knowledge).
- In two terminal windows, run `./proxy <port>` and `telnet localhost <port>`, where `<port>` is the user-defined port number.
- In the telnet terminal, copy and paste the contents of `telnet_input.txt` and press enter(Or, enter input in another fashion you may have). The request is now processed by the proxy server.
 
