# Chatting Application [Java]

## Abstract

Teleconferencing or chatting refers to any kind of communication that offers a real-time transmission of messages from sender to the receiver. Chatting is a method of using technology to bring people and ideas together despite geographical barriers. The technology to provide the chatting facility has been available for years, but acceptance is quite recent. Analysis of chatting provides an overview of the technologies used, available features, functions, system architecture, and database structure of an Instant Messaging application: IChat (IC). The objective of the IC application is to facilitate text messaging, group chatting options, and data transfer without size restriction, which is commonly seen in most messaging applications.

---

## Introduction

The Chatting Application is a desktop-based application. This client-server chat application is based on Java Swing and uses the socket package. It's simple, easy, and requires only core Java knowledge. The application is a good example of using `java.io` and `java.net` packages to create a chat application. A beginner in Java who is familiar with these packages can benefit from this project.

Chatting is a method of using technology to bring people and ideas together despite geographical barriers. The technology has been available for years, but acceptance was quite recent. Our project is an example of a multiple client chat server. It is made up of two applications: the client application, which runs on the user’s PC, and the server application, which runs on any PC on the network. To start chatting, the client should connect to the server. We will focus on TCP and UDP socket connections, which are a fundamental part of socket programming.

**Keywords**: sockets, client-server, Java network programming, socket functions, multicasting, etc.

---

## Main Objective

The aim of this project is to implement a simple chat application between a server and a client. The application is desktop-based and implemented using Swing and AWT. The project is developed in Java SE language and executed on a single stand-alone Java application across a network using the loopback address concept.

The application consists of two programs:
- Server
- Client

### Server

The server module of the application waits for the client to connect to it. Once a connection is granted, the client interacts, communicates, and connects to the server, allowing mutual communication. The server's duty is to let clients exchange messages.

### Client

The client module sends requests to the server. The user utilizes the client to connect to the server. Once the connection is established, the user can communicate with the connected server.

---

## Requirements

### External Interface Requirements

#### User Interface
The user interface required to be developed for the system should be user-friendly and attractive. There are two sets of Java APIs for graphics programming: AWT (Abstract Windowing Toolkit) and Swing.
- **AWT**: Introduced in JDK 1.0. Most AWT components have become obsolete and should be replaced by newer Swing components.
- **Swing**: A comprehensive set of graphics libraries that enhance AWT, introduced as part of Java Foundation Classes (JFC) after JDK 1.1. JFC includes Swing, Java2D, Accessibility, Internationalization, and Pluggable Look-and-Feel Support APIs. JFC has been integrated into core Java since JDK 1.2.

### Software Interfaces

- **Programming Language**: Java and Socket Programming

### Operational Concepts and Scenarios

The operation of the application is based on the inputs given by the user:
- When the run button is clicked, the chat form is initialized with a connection between the host and the client machine.
  - The server must be started first before a client starts.
  - Contains a rich textbox to send messages from one user to another.
  - Contains a textbox for messages to be written and sent across the network.
  - Contains a Send button.
  - When the send button is clicked, the text in the textbox is encoded and sent as a packet over the network to the client machine. Here, the message is decoded and shown in the rich textbox.

---

## Project Scope

This project can be mainly divided into two modules:
1. Server
2. Client

This project is mainly dependent on the client/server model. The client requests the server, and the server responds by granting the client's request. The proposed system should provide the above features along with the following ones:

### Server
A server is a computer program that provides services to other computer programs (and their users) in the same or other computers. The computer that a server program runs on is also frequently referred to as a server. The server is always waiting for client requests. The client comes and goes, but the server remains the same. A server application normally listens to a specific port waiting for connection requests from a client. When a connection request arrives, the client and server establish a dedicated connection over which they can communicate.

### Client
On the client side, the client knows the hostname of the machine on which the server is running and the port number on which the server is listening. To make a connection request, the client tries to rendezvous with the server on the server's machine and port. The client also needs to identify itself to the server, so it binds to a local port number that it will use during this connection.

The model used for this project is the single server–single client model. The following specifications must be implemented:
1. The server and client are two separate programs.
2. The client screen.
3. The client-server screen.

---

## Future Work

There is always room for improvement in any software package, however good and efficient it may be. The most important thing is to be flexible to accept further modifications. Currently, we are just dealing with text communication. In the future, this software may be extended to include features such as:
- File transfer: This will enable the user to send files of different formats to others via the chat application.
- Voice chat: This will enhance the application to a higher level where communication will be possible via voice calling, similar to a telephone.
- Video chat: This will further enhance the feature of calling into video communication.

---

## Conclusion

We developed network applications in Java using sockets, threads, and Web services. These software applications are portable, efficient, and easily maintainable for a large number of clients. Our developed web-based chatting software is unique in its features and, more importantly, easily customizable. The `java.net` package provides a powerful and flexible set of classes for implementing network applications. Typically, programs running on client machines make requests to programs on a server machine. These involve networking services provided by the transport layer. The most widely used transport protocols on the Internet are TCP (Transmission Control Protocol) and UDP (User Datagram Protocol).

- **TCP**: A connection-oriented protocol providing a reliable flow of data between two computers.
- **UDP**: A simpler message-based connectionless protocol that sends packets of data known as datagrams from one computer to another with no guarantees of arrival.

---
