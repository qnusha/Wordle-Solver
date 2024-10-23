Using TCP Socket Programming to solve a wordle riddle

Approach:
I wrote this program in Python. The program will run on a given port and host and build a socket connectiion tot he FTP server. Based on what the command script specifies, we added functionality for removing, copying, moving, files and directions, as well as list your directory for degbbing. After connecting to the server using a TCP socket, and a customized username and password, we can perform one operation relating to the FTP.

<!-- reads command script and parse urls in this format: 
ftp://[USER[:PASSWORD]@]HOST[:PORT]/PATH -->
I perform a basic strategy to implement a command line file system functionality. I Take in a path, username, and password. I thought it would not be was not too difficult since the file system already gives their own versions OOD. Once the operation functionality is working, we are able to do more creative operations such as copy and move, that uses a mixture of delete, upload, and download to make these directories and files.

Challenges:
A challenge I faced was testing and debugging my program, I had a very hard time figuring out how to read through bytes until the end of a file. This made it difficult trying to handle very big files. I also struggled with storing the word bank as a global variable, as this later made it difficult to reassign the variable in functions. 

Testing:
I tested my code with lots of print statements and responses of data that was recieved. In order to find out how all the methods are interacting with eachother, and I would print them out after each guess message sent. I would print every message and data recieved from the server in order to understand how it is being give to us. I also tested different command scripts on both the vscode terminal as well as my desktop terminal.
