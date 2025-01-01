# SignalR 

This project is a (very) basic introduction to SignalR that allows real-time communication testing using WebSockets.

## Testing
1. Install this project (.NET 7) and Postman;
2. Execute this project;
3. Open Postman > File > New > WebSocket;
4. Enter the URL, with a "ws" prefix for unsecured connection or "wss" for secured, and the route "chat-hub" that is specified in Program.cs, example: ```ws://localhost:5192/chat-hub```
5. Enter handshake message (the ASCII Record Separator  is required to signal the end of the handshake): ```{"protocol":"json","version":1}```
6. Click on Connect and Send;
7. Enter the invocation message (you can type anything instead of "Test message"): ```{"arguments":["Test message"],"invocationId":"0","target":"SendMessage","type":1}```
8. Click on Send.

<br>

Tutorial followed: <a href="https://www.youtube.com/watch?v=9_pRk7PwkpY">Building Real-Time Applications With SignalR & .NET 7</a> by Milan Jovanovic.
