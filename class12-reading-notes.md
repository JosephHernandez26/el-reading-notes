# El Reading Notes of the 401 Variety

## Class 12 reading notes

### El Questions

#### 1. What is the benefit of transforming data into packets?

- Packets split the data in order for it to be processed more efficiently which in turn makes sending the data much faster.

#### 2. UDP is often refereed to as a connection-less protocol. Why is this?

- A UDP does not require a connection be established between the source and destination to transmit data.

#### 3. Can a socket server application have multiple socket connections?

- Yes, tt is possible to have multiple TCP sockets listen on the same port connection.

#### 4. Can a socket connection application be connected to multiple socket servers?

- Yes.

#### 5. Can an application be both a socket server and a socket connection?

- It is not necessary. But if you want to have a "peer-to-peer" type system, then you just have each client run both a client and a server socket - the server socket for accepting connections from other clients and the client socket for establishing connections to others..

### Document the following Vocabulary Terms

**Observer Pattern**

> The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

**Listener**

> Listens for a specific event to be logged.

**Event Handler**

> Logs when an event is triggered, runs callback function if such a function is provided.

**Event-Driven Programminmg**

> Programming that is "driven" by events. Functions don't run unless events are triggered.

**Event Loop**

> The event loop is referred to as the message dispatcher, message loop, message pump, or run loop. The event loop is a programming construct or design pattern that waits for and dispatches events or messages in a program.

**Event Queue**

> An event queue is a repository where events from an application are held prior to being processed by a receiving program or system.

**Call Stack**

> A call stack is a stack data structure that stores information about the active subroutines of a computer program.

**Emit/Raise/Trigger**

> Triggers an event after an action occurs.

**Subscribe**

> Signing up (subscribing) to receive a product regularly.

**Database**

> Collection of dataDescribe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server.

 <a href="#top">Take Me To The Repo!!</a>
 