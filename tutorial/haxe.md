---
title: "Haxe Framework"
library_lang: "haxe"
---
{% include 'tutorial_intro.md' %}

### Prerequisites
* Thrift requires at least Haxe 3.1.3. (You may try with older versions on your own luck).

### Client 
For this tutorial, we put both the server and the client main code into one single program. 
Depending on the arguments passed, it runs as a server or as a client program.

[snippet:path=tutorial/haxe/src/Main.hx:lines=20,332]

Were done with the client, but need some more for the server: A service handler implementaion.
  
### Server
As the name suggests, the service handler implements the Thrift service on the server side. 
The code to achieve this is as follows:

[snippet:path=tutorial/haxe/src/CalculatorHandler.hx:lines=20,102]

### Additional Information

Similar to Thrift, Haxe supports different compiler targets. Depending on the target, some features 
may or may not be supported. For example, if you plan to use Flash or JavaScript targets, 
there is currently no way to pass command line arguments to the program.
