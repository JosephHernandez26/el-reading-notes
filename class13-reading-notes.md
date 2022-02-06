# El Reading Notes of the 401 Variety

## Class 13 reading notes

### El Questions

#### 1. What does it mean that web sockets are bidirectional? Why is this useful?

- Bi-directional means information is sent in both directions. Think `response` `request` data flow.

#### 2. Does socket.io use HTTP? Why?

- Socket.io is created in a way to allow HTTP and websocket servers to co-exist on the same port location.

#### 3. What happens when a client emits an event?

- The server 'subscribes' to it and is able to be triggered.

#### 4. What happens if a client “misses” an event?

- Packets are dropped and data is lost.

#### 5. How can we mitigate this?

- Drop or eliminate the use of old sockets.

### Document the following Vocabulary Terms

**Socket**

> An instance of a client connected to a server.

**Web Socket**

> This is a computer communications protocol. AKA a way a computer has of communicating information between multiple servers & clients.

**Socket.io**

> Real-time bidirectional and event-based communication for sending multiple events across multiple servers & clients.

**Client**

> This is one application that is connected to one or multiple servers.

**Server**

> These are the data/information-centers that connect multiple clients to each other or deal with responding to a request.

**OSI Model**

> This is the 7 layer model of explaining the functions of a networking system.

**TCP Model**

> This is a more concise version of the OSI model, consisting of only 4 layers.

**TCP**

> Transmission Control Protocol - The transport protocol that is used

**UDP**

> User Diagram Protocol - The communications protocol that is used for establishing low-latency and loss-tolerating connections between applications on the internet.

**Packets**

> These are the raw data send between connections that the headers tells to reconstruct properly into the data.

 <a href="#top">Take Me To The Repo!!</a>