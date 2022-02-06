# El Reading Notes of the 401 Variety

## Class 14 reading notes

### El Questions

#### 1. What’s the difference between a FIFO and a standard queue?

- A FIFO queue hold messages in a strictly defined order of First In First Out, while a standard queue only holds a reference to messages either by name or id.

#### 2. How can the server be assured a message was properly received?

- It will receive a receipt, of sorts, from the source receiving the message. Similar to the idea of a 'read' receipt.

#### 3. What classic design pattern is best represented by event driven programming?

- The pub/sub pattern.

#### 4. How do you test an event driven system?

- Through testing each individual event using unit tests.

### Document the following Vocabulary Terms

**FIFO Queue**

> A FIFO queue is a queue that operates on a First-In, First-Out (FIFO) principle. This means that the request (like a customer in a store or a print job sent to a printer) is processed in the order in which it arrives.

**Pub/Sub**

> Pub means 'publish,' in event driven programming, to emit an event, is to publish it for the server and clients to hear (subscribe to).
> Sub means 'subscribe, and this happens when the server and/or clients are listening for a published event, they are 'subscribed.'

 <a href="#top">Take Me To The Repo!!</a>
 