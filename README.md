# File-Transfer

# ABSTRACT
FTP (File Transfer Protocol) is a network protocol for transmitting files 
between computers over Transmission Control Protocol/Internet Protocol 
(TCP/IP) connections. 
Within the TCP/IP suite, FTP is considered an application layer protocol. The 
end user's computer is typically called the local host. The second computer 
involved in FTP is a remote host, which is usually a server. Both computers 
need to be connected via a network and configured properly to transfer files 
via FTP. 

# SCOPE OF THE PROJECT 
Socket programming is important to understand how internet based inter 
process communication work. Socket programming shows how to use socket 
APIs to establish communication links between remote and local processes. 
Using FTP file exchange between client and server is easier to do because the 
communication is done directly without going through an intermediary, for 
communication using FTP need to be designed an application that allows 
communication between the client and server directly without using the
browser.

# PROJECT DESCRIPTION

PROJECT DESCRIPTION
In Client-Server programming there are two different programs or process, 
one which initiates communication called Client process and other who is 
waiting for communication to start called Server process. 
In the implementation, we have a client side and a server side. The server 
and client have two different programs that are run in different directories.
The client read a file and send its data to server. The server then receives 
the data and write it in a text file. 
The client-side implementation of socket-based File Transfer Protocol in C: 
The functions used are: 
1) File_exist() – The function is of datatype ‘int’ and takes the character 
array including the filename as the parameter. The function is used to 
determine if the file that has to be transferred exists. It uses string 
comparision to compare the name of the file present in the directory to 
the file name entered by the user. 
2) Send_file() – The function is of datatype ‘int’ and takes the socket 
number and the character array including the verified filename as the 
parameters. The function is used to send a file to the server directory. In 
order to do this, the contents of the file that has to be transferred is read 
and then concatenated to the file path of the server directory. 
3) Put_file ()- The function is of datatype ‘void’ and takes the client 
socket number and the character array including the verified filename 
as the parameters. The function is used to verify if the file has been 
transferred to the server’s directory. The verification is done using a 
sequence of if else ladders. The options for overwriting the already 
existing file is included as well. 
4) Get_file()-The function is of datatype ‘void’ and takes the accepted 
socket number and the character array including the verified filename as the parameters. The function is used to indicate the completion of the 
utilization of the file transfer protocols. 
The server-side implementation of socket-based File Transfer Protocol in 
C: 
The implementation of the server side includes the same functions as the 
client with varying file paths and socket numbers. 
Main ()-Along with the basic declarations and configurations, the server 
side implementation includes aa while loop for accepting connections from 
the client side.

![image](https://github.com/Meenalbagare/File-Transfer/assets/99323366/c118f429-a57d-4b38-a01d-9741b3f7b57c)

![image](https://github.com/Meenalbagare/File-Transfer/assets/99323366/60d8846b-18c0-4757-b839-3e073fe2654e)

# CONCLUSION 
Implementing file transfer using socket programming In C language provides a 
reliable and efficient way to transfer data between networked computers. The use of 
sockets enables the creation of a connection between a client and a server, allowing 
the transfer of files of any size and type. C language provides powerful and flexible 
functions for working with sockets, which can be customized to meet specific 
requirements. 
Socket programming in C language is a widely used and tested method for file 
transfer in computer networks.It provides a low-level approach that allows 
developers to have complete control over the transfer process, making it ideal for 
implementing high-performance file transfer systems


