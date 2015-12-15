# TCPSockets
TCPSockets example: An activity that reqires information, should through composition (over inheritance) use a service e.g IBService with a Task<string> GetStatus(int userId), in our case an implementation of IBService could be BServiceWithTcpConnector : IBService, in which the implementation would use a TcpClient. In doing so we are repsecting the Single Responsibility i.e the class/activity using the IBService would not have to change if the implementation became BServiceWithHttpConnector : IBService, or an other implpementation.

By splitting out this concern, we can load test the external service without conerning ourselves with any calling code, hence achieving / demosntrating loose coupling.

Finally, the abstracionts would be sealed classes, ultimately TcpClient wrappers should not be changed through inheritance.

   

