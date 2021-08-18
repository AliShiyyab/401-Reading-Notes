# WebSocket 

>In the specifice state : **You will build a server that accepts a message that carries a user’s name. In response, the server will push a greeting into a queue to which the client is subscribed.**

>In General : **Massenger system between followers**

>Edited on depandicies and other places to can be worked as a socket system.

>You need to create some classes like massege and whats content of masseges.

>Create a `@MessageMapping("/Example")  @SendTo("/topic/greetings")` in the constroller

>The `@MessageMapping` annotation ensures that, if a message is sent to the `/Example` destination, the `greeting()` method is called.

>I need to git the full descripe of this subject in the lecture
