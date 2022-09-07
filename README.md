# Fight Arena
## CSD-D JQR Project v. 1
### September 7th, 2022

<br>

# 1. Introduction
## 1.1 Overview

Fight Arena serves as a project to determine a Trainee's ability to understand and implement various requirements of the Developer JQR. You, the Trainee, are tasked with creating a gaming system that includes five (5) modules; Data structures, a Server, Clients, Workers, and Testing and Documentation.

- Data Structures: Data structures will be written in the C language and adhere to the BARR-C style Guide. The data structures written will be used for the various components in the Server, Clients, and Workers. 

- Server: The server will be written in the C language and adhere to the BARR-C style guide. It is responsible for handling client connections, managing fighters in an arena, distributing work to workers, and supplying fight results to clients. 

- Clients: Clients will have two versions; one written in the C language and one written in Python. They will adhere to the BARR-C and Google style guides, respectively. The client is responsible for providing a user interface, communicating with the server, and displaying fighter results. 

- Workers: Workers will have two versions; one written in the C language and one written in Python. They will adhere to the BARR-C and Google style guides, respectively. The worker is responsible for finding a server to obtain work, calculating fight results, and returning results to the server. 

- Testing and Documentation: Testing and documentation will be performed by the Trainee. Testing will fully test all aspects of every module and their interoperability. Documentation will serve as a setup guide and user guide.

The project will happen in four (4) Phases: 
1. Data Structures 
2. Server Creation 
3. Client Creations  
4. Worker Creations

> Testing and Documentation will occur during every phase of the project. Phases are designed to build on previous phases. A Trainee cannot move onto the next phase until they have completed the current phase and been approved by a designated Trainer.

<br>

## 1.2 Administrative
### 1.2.1 Time Considerations

This project is designed to adhere to the six month (180 day) standard of completing the JQR. A rough timeline of completing each module is as follows: 

- Data Structures: two to three months
- Server: three (3) weeks to six (6) weeks 
- Clients: two (2) weeks to one (1) month 
- Workers: two (2) weeks to one (1) month 

<br>

# 2 Detailed Requirements

## 2.1 Data Structures

Data structures are C language modules created to be used as a library for various components during follow-on phases. Each data structure should be data type agnostic, meaning they can handle data given to it. They should be designed in a finite way; finite inputs and outputs. 

Data Structures may be completed in any order; data structures may be used to build other data structures. Data structures that should be created are as follows:

<br>

### 2.1.1 Arrays

|Req. |Summary |
|-|-|
|2.1.1.1 |Correctly creates an array context |
|2.1.1.2 |Can hold any data type in the array |
|2.1.1.3 |Can return the size of the array |
|2.1.1.4 |Can add an element to the end of the array |
|2.1.1.5 |Can add an element to the beginning of the array |
|2.1.1.6 |Can insert an element anywhere within the array |
|2.1.1.7 |Can remove an element from the end of the array |
|2.1.1.8 |Can remove an element from the beginning of the array |
|2.1.1.9 |Can remove an element anywhere within the array |
|2.1.1.10 |Can get an element from n position within the array |
|2.1.1.11 |Can destroy all elements within an array using the correct deallocation function |
|2.1.1.12 |Can correctly destroy an array context |
|2.1.1.13 |Causes no memory leaks during all operations|

<br>

### 2.1.2 Multi-dimensional Arrays

> This module is conducive to building on the 'Array'

|Req. |Summary |
|-|-|
|2.1.2.1 |Correctly creates a multi-dimensional array context |
|2.1.2.2 |Can hold any data type in the multi-dimensional array |
|2.1.2.3 |Can return the size of the multi-dimensional array |
|2.1.2.4 |Can add an array to the end of the multi-dimensional array |
|2.1.2.5 |Can add an array to the beginning of the multi-dimensional array |
|2.1.2.6 |Can insert an array anywhere into the multi-dimensional array |
|2.1.2.7 |Can remove an array from the end of the multi-dimensional array |
|2.1.2.8 |Can remove an array from the beginning of the multi-dimensional array |
|2.1.2.9 |Can remove an array anywhere in the multi-dimensional array |
|2.1.2.10 |Can get an array at n position within a multi-dimensional array |
|2.1.2.11 |Can get an element at (n,n) position within a multi-dimensional array |
|2.1.2.12 |Can destroy all arrays within a multi-dimensional array using the correct deallocation functions |
|2.1.2.13 |Can correctly destroy a multi-dimensional array context |
|2.1.2.14 |Causes no memory leaks during all operations|

<br>

### 2.1.3 Circularly Linked List

|Req. |Summary |
|-|-|
|2.1.3.1 |Correctly creates a circularly linked list context |
|2.1.3.2 |Can hold any data type in the circularly linked list |
|2.1.3.3 |Can return the size of the circularly linked list |
|2.1.3.4 |Can add an element to the beginning of a circularly linked list |
|2.1.3.5 |Can add an element to the end of a circularly linked list |
|2.1.3.6 |Can insert an element anywhere into a circularly linked list |
|2.1.3.7 |Can remove an element from the beginning of a circularly linked list |
|2.1.3.8 |Can remove an element from the end of a circularly linked list |
|2.1.3.9 |Can remove an element from anywhere within a circularly linked list |
|2.1.3.10 |Can get an element at the n position of a circularly linked list |
|2.1.3.11 |Can destroy all elements within a circularly linked list using the correct deallocation functions |
|2.1.3.12 |Can correctly destroy a circularly linked list context |
|2.1.3.13 |Causes no memory leaks during all operations |
|2.1.3.14 |Can find the first occurrence of an item in a circularly linked list |
|2.1.3.15 |Can sort a circularly linked list alphanumerically given a function pointer (sorting function)|

<br>

### 2.1.4 Queue 
|Req. |Summary |
|-|-|
|2.1.4.1 |Correctly creates a queue context |
|2.1.4.2 |Can hold any data type in the queue |
|2.1.4.3 |Can return the size of the queue |
|2.1.4.4 |Can return a Boolean determining if the queue is empty |
|2.1.4.5 |Can enqueue an item into the queue |
|2.1.4.6 |Can dequeue an item from the queue |
|2.1.4.7 |Can peek at the top item in the queue |
|2.1.4.8 |Can destroy items in a queue using the correct deallocation functions |
|2.1.4.9 |Can correctly destroy a queue context |
|2.1.4.10 |Causes no memory leaks during all operations|

<br>

### 2.1.5 Priority Queue 
|Req. |Summary |
|-|-|
|2.1.5.1 |Correctly creates a priority queue context |
|2.1.5.2 |Can hold any data type in the priority queue |
|2.1.5.3 |Can return the size of the priority queue |
|2.1.5.4 |Can return a Boolean determining if the priority queue is empty |
|2.1.5.5 |Can properly enqueue an item priority queue based on the item's given priority |
|2.1.5.6 |Can dequeue an item from the priority queue |
|2.1.5.7 |Can destroy items in a priority queue using the correct deallocation functions |
|2.1.5.8 |Can correctly destroy a priority queue context |
|2.1.5.9 |Causes no memory leaks during all operations|

<br>

### 2.1.6 Stack 
|Req. |Summary |
|-|-|
|2.1.6.1 |Correctly creates a stack context |
|2.1.6.2 |Can hold any data type in the stack |
|2.1.6.3 |Can return the size of the stack |
|2.1.6.4 |Can return a Boolean determining if the stack is empty |
|2.1.6.5 |Can push an item to the top of the stack |
|2.1.6.6 |Can pop an item from the top of the stack |
|2.1.6.7 |Can peak at the item on the top of the stack |
|2.1.6.8 |Can destroy all items on the stack using the correct deallocation functions |
|2.1.6.9 |Can correctly destroy a stack context |
|2.1.6.10 |Causes no memory leaks during all operations|

<br>

### 2.1.7 Tree 
|Req. |Summary |
|-|-|
|2.1.7.1 |Correctly creates a tree context |
|2.1.7.2 |Can hold any data type in a tree |
|2.1.7.3 |Can find the first occurrence of an item in a tree |
|2.1.7.4 |Can insert an item into a specified location in a tree |
|2.1.7.5 |Can remove an item from a specified location in a tree |
|2.1.7.6 |Can destroy all items on the stack using the correct deallocation functions |
|2.1.7.7 |Can correctly destroy a tree context |
|2.1.7.8 |Causes no memory leaks during all operations|

<br>

### 2.1.8 Binary Search Tree 
|Req. |Summary |
|-|-|
|2.1.8.1 |Correctly creates a binary search tree context |
|2.1.8.2 |Can hold any data type in a binary search tree |
|2.1.8.3 |Can perform depth first traversal in a binary search tree |
|2.1.8.4 |Can perform breadth first traversal in a binary search tree |
|2.1.8.5 |Can locate an item in a binary search tree |
|2.1.8.6 |Can add an item to a binary search tree |
|2.1.8.7 |Can remove an item from a binary search tree |
|2.1.8.8 |Can destroy all items in a binary search tree using the correct deallocation functions |
|2.1.8.9 |Can correctly destroy a binary search tree context |
|2.1.8.10 |Causes no memory leaks during all operations|

<br>

### 2.1.9 Weighted Graph 
|Req. |Summary |
|-|-|
|2.1.9.1 |Correctly creates a weighted graph context |
|2.1.9.2 |Can hold any data type in a weighted graph |
|2.1.9.3 |Can define structures required for a weighted graph |
|2.1.9.4 |Can create a weighted graph with n number of nodes |
|2.1.9.5 |Can add n number of edges to a weighted graph |
|2.1.9.6 |Can find a node within an existing weighted graph |
|2.1.9.7 |Can find an edge within a weighted graph |
|2.1.9.8 |Can remove an edge from a weighted graph |
|2.1.9.9 |Can remove a node and all its edges from a weighted graph |
|2.1.9.10 |Can calculate the weight of a path within a weighted graph |
|2.1.9.11 |Can destroy all edges and nodes within a weighted graph using the correct deallocation functions |
|2.1.9.12 |Can correctly destroy a weighted graph context |
|2.1.9.13 |Causes no memory leaks during all operations|

<br>

### 2.1.10 Hash Table 
|Req. |Summary |
|-|-|
|2.1.10.1 |Correctly creates a hash table context |
|2.1.10.2 |Can hold any data type in a hash table |
|2.1.10.3 |Can navigate through a hash table to find the nth item |
|2.1.10.4 |Can find an item in a hash table |
|2.1.10.5 |Can remove selected items from a hash table |
|2.1.10.6 |Can insert an item into a hash table |
|2.1.10.7 |Can implement functionality to mitigate hash collisions within a hash table |
|2.1.10.8 |Can destroy all items in a hash table using the correct deallocation functions |
|2.1.10.9 |Can correctly destroy a hash table context |
|2.1.10.10 |Causes no memory leaks during all operations|

<br>

### 2.1.11 Thread Pool 
|Req. |Summary |
|-|-|
|2.1.11.1 |Correctly creates a thread pool context |
|2.1.11.2 |Can create a pool of worker threads that accept a job function pointer and arguments |
|2.1.11.3 |Can implement a queue to hold received jobs |
|2.1.11.4 |Can gracefully tear down when stop signal received |
|2.1.11.5 |Can destroy all jobs in a thread pool using the correct deallocation functions |
|2.1.11.6 |Can correctly destroy a thread pool context |
|2.1.11.7 |Causes no memory leaks during all operations|

## 2.2 Server

- Written in the C language and adheres to the BARR-C style guide 

- Handles client connections 

- Manages fighters in an arena 

- Distributes work to workers 

- Supplies fight results to clients 

- Establishes connections with clients on one TCP port 

- Listens for new workers on a UDP port. Once a broadcast request from a worker is received on that port, communications change to TCP on the same port number. 

- Started via command line with two flags 
    - `-c` – Configuration file
    - `-l` – Log file

<br>

### 2.2.1 Server Startup

The server will be started via the command line with two (2) flags. The first flag is `-c` and the argument given is the name of a configuration file (see 2.2.1.1 for details). The second flag is `-l` and the argument given is the name of a log file (see 2.2.1.2 for details). 

Example command: `./fight_arena –c config.txt -l log_file.txt`

<br>

#### 2.2.1.1 The Configuration file 

The format of the configuration file and filename is up to the Trainee. How the file is parsed and ingested by the Server is also up to the Trainee. The information that must be present in the configuration file is as follows: 

- Client listening port: TCP port the server listens on for clients 

- Worker listening port: TCP and UDP port the server listens on for workers 

- Session ID timeout: Number of seconds that a session ID is valid 

- Max client count: Maximum amount of session IDs that can be active.

<br>

#### 2.2.1.2 The Log File 

The format of the log file and filename is up to the Trainee. How the server adds entries to the file is up to the Trainee as well. The information that must be present in a log entry is as follows: 

- Event timestamp
- Event type
- Event sub-type (optional)
- Event success or failure
- Example: `2022090814:13:20 Connection 172.168.0.12:12345 Success`

### 2.2.2 Server Functionality 

<br>

#### 2.2.2.1 Client Management and the fight arena 

- When a client sends a fighter request, and the fighter data is valid, the server will place this fighter into a fight arena. 
- The server will then wait up to 30 seconds for another fighter request to come in. 
    - If another client sends in a fighter request,  
        - If it is a valid fighter packet it is placed into the same fight arena 
        - otherwise, the server continues waiting 
    - If 30 seconds have elapsed, then the server will create a bot fighter and place them into the arena 
- After two fighters are in the arena, the server packages them up to send to a Worker for fight processing 
- The server sends this data to a Worker to get the fight results 
- The server sends a 'Fighter Response' packet to all clients with the winning fighter 
- It is up to the Trainee how to track Client connections internally, and how to correspond a connection with a fighter

<br>

#### 2.2.2.2 Worker Management 
- The Server should maintain a pool of available Workers 
- As workers are discovered, they should be added to this pool 
- When Workers do not respond to 'Work Awake' packets, they should be removed 
- The Trainee is responsible for designing how the server handles active and inactive workers and how it stores worker information 
- The Trainee is responsible for how the server decides which worker to use when there is work to be done 

<br>

### 2.2.3 Server-Client Communication Protocols 

<br>

#### 2.2.3.1 Client connecting to Server 
- 'Connect Request' is how a client gets a valid Session ID 
- A client sends a 'Connect Request' to a designated TCP port 
- If the server can accept clients, it will respond with a 'Connect Response' packet containing the new Session ID 
- If the server cannot accept new clients, it will respond with a 'Failure' packet with a 'server busy' opcode. 
- The client will terminate the connection

<br>

#### 2.2.3.2 Client Sending Fighter 
- the server will listen on a defined TCP port for connections from clients.  
- Clients must have a valid Session ID to send fighters.  
    - This is done by a client sending a 'Connect Request' packet (protocol defined in section 2.2.3.1). 
- Client will send a 'Fighter Request' packet containing all the details of a fighter 
- If fighter data is valid and after the fight statistics have been calculated, the server will respond with a 'Fighter Acknowledge' packet containing fight results 
- If the given session ID is invalid, the Server will respond with a 'Failure' packet with 'Invalid Session ID' opcode 
- If there is a general error (server error or calculation error), the Server will respond with a 'Failure' packet with a 'Server-Side Error' opcode 
- If a client has sent a fighter packet with invalid fighter stats, the Server will respond with a 'Fighter Reject' packet with appropriate opcode 

<br>

### 2.2.4 Server-Worker Communication Protocol 

<br>

#### 2.2.4.1 Worker Discovering a Server 
- The server will listen on a defined UDP port for 'Discovery Request' packets from potential workers 
- Once a packet is received, the Server will send a 'Discovery Response' packet to the TCP port identified by the Worker's request packet. 
- If the worker responds with a 'Discovery Acknowledge' packet, the server will send a 'Discovery Acknowledge' packet. 
- If the worker responds with a 'Discovery Reject' packet, the server ignores the request 
- The server terminates the connection 

<br>

#### 2.2.4.2 Server giving Worker work 
- Server identifies which of its available Workers can take work 
- Server sends a 'Work Awake' packet to the Worker. 
- If Worker never responds 
    - Server terminates connection (Should remove worker from worker pool) 
- Worker responds with 'Work Awake' packet 
- Server sends a 'Work Data' packet 
- Worker processes data 
- Worker sends a 'Work

<br>

## 2.3 Client 

<br>

## 2.4 Worker 

<br>

## 2.5 Detailed Packet Requirements

<br>

### 2.5.1 Packet Type codes 

|||
|-|-|
|Connect|0x01|
|Fighter|0x02|
|Discovery|0x03|
|Work|0x04|
|Failure|0xFF|

<br>

### 2.5.2 Opcodes 
|||
|-|-|
|Server Busy|0x00|
|Session ID|0x01|
|Invalid Session ID|0x02|
|Server Error|0x03|
|Fight Results|0x04|
|Request|0x05|
|Response|0x06|
|Reject|0x07|
|Acknowledge|0x08|
|Awake|0x09|
|Data|0x0a|

<br>

### 2.5.3 Connect Packets 

Connect Packets are how Clients can retrieve a new Session ID. 

<br>

#### 2.5.3.1 Connect Request: 

<br>

#### 2.5.3.2 Connect Response:

<br>

### 2.5.4 Fighter Packets 

Fighter Packets are used for Client and Server communications for sending fighter information, and retrieving fight results or errors 

<br>

#### 2.5.4.1 Fighter Request 
The Fighter Request packet will consist of 8 fields: 
1. Fighter Packet Flag – 1 Byte 
2. Request Flag – 1 Byte 
3. Session ID – 8 Bytes 
4. Fighter Attack Stats – 1 Byte 
5. Fighter Defense Stats – 1 Byte 
6. Fighter Luck Stats – 1 Byte 
7. Fighter Name Length (Number of characters in fighter name) – 1 Byte 
8. Fighter Name – Variable length

<br>

#### 2.5.4.2 Fighter Acknowledge 
1. The Fighter Acknowledge will consist of 8 fields: 
2. Fighter Packet Flag – 1 Byte 
3. Acknowledge Flag – 1 Byte 
4. Did Win Flag – 1 Byte. 0x01 if Client won, 0x00 if Client lost 
5. Opponent Attack stat – 1 Byte 
6. Opponent Defense stat – 1 Byte 
7. Opponent Luck stat – 1 Byte 
8. Opponent Name Length – 1 Byte 
9. Opponent Name – Variable length

<br>

#### 2.5.4.3 Fighter Reject 

The Fighter Reject packet will consist of three fields: 
1. Fighter Packet flag – 1 Byte 
2. Reject Flag – 1 Byte 
3. Reason Code – 1 Byte (See below for reason codes) 

Reject Reason Codes: 
|||
|-|-|
|Name Characters|0x01|one or more bytes in name are not in the ASCII Range|
|Name Len|0x02|The name is either too short or too long|
|Attack Value|0x03|The attack value is either below 10 or above 80|
|Defense Value|0x04|The defense value is either below 10 or above 80|
|Luck Value|0x05|The luck value is either below 10 or above 80|
|Final Value|0x06|The total value of attack, defense, and luck does not equal 100|

<br>

### 2.5.5 Discovery Packets 

Discovery packets are used for Workers to be able to find a Fight Arena server. 

<br>

#### 2.5.5.1 Discovery Request 

The Discovery Request packet consists of 4 fields: 
1. Discovery Packet flag – 1 Byte 
2. Request flag – 1 Byte 
3. Worker's IP Address – 4 Bytes 
4. Worker's TCP port – 1 Byte 

<br>

#### 2.5.5.2 Discovery Response 

The Discovery Response packet consists of 3 fields: 
1. Discovery Packet flag – 1 Byte 
2. Response flag – 1 Byte 
3. Server's IP – 4 Bytes 

<br>

#### 2.5.5.3 Discovery Acknowledge 

The Discovery Acknowledge packet consists of 2 fields: 
1. Discovery Packet flag – 1 Byte 
2. Acknowledge flag – 1 Byte 

<br>

#### 2.5.5.4 Discovery Reject 

The Discovery Reject packet consists of 2 fields: 
1. Discovery Packet flag – 1 Byte 
2. Reject flag – 1 Byte 

<br>

### 2.5.6 Work Packets 

Work packets are used by the Server to send work to Workers and for Workers to return results to the Server. 

<br>

#### 2.5.6.1 Work Awake 

The Work Awake packet consists of 2 fields: 
1. Work Packet flag – 1 Byte 
2. Awake flag – 1 Byte 

<br>

#### 2.5.6.2 Work Data 

The Work Data packet consists of 8 fields: 
1. Work Packet flag – 1 Byte 
2. Data flag – 1 Byte 
3. Fighter 1 Attack stat – 1 Byte 
4. Fighter 1 Defense stat – 1 Byte 
5. Fighter 1 Luck stat – 1 Byte 
6. Fighter 2 Attack stat – 1 Byte 
7. Fighter 2 Defense stat – 1 Byte 
8. Fighter 2 Luck stat – 1 Byte 

<br>

#### 2.5.6.3 Work Response 

The Work Response packet consists of 3 fields: 
1. Work Packet flag – 1 Byte 
2. Response flag – 1 Byte 
3. Return Code – 1 Byte (see below for return codes) 

Return Codes: 
|||
|-|-|
|Fighter 1 Wins|0x01|
|Fighter 2 Wins|0x02|
|Error|0xFF|

<br>

### 2.5.7 Failure Packet 

The Failure Packet consists of 2 fields: 
1. Failure Packet flag – 1 Byte 
2. Opcode – 1 Byte (See section 2.5.2 for opcodes) 

<br>

# 3 Trainers and Grading 