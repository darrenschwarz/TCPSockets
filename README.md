# TCPSockets
TCPSockets example: An activity that reqires information, should through composition (over inheritance) use a service e.g IBrambleService with a Task<string> GetStatus(int userId), in our case an implementation of IBrambleService could be BrambleServiceWithTcpConnector : IBrambleService, in which the implementation would use a TcpClient.  

