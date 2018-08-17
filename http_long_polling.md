# What is HTTP Long Polling?

Web applications were originally developed around a client/server model, where the Web client is always the initiator of transactions, requesting data from the server. Thus, there was no mechanism for the server to independently send, or push, data to the client without the client first making a request.

> web application是围绕client/server模型来构造的。  
> 在web client和web server交互的过程中，只能由web client充当发起者。  
> 也就是说，如果web client不发起请求，web server是没有办法主动的向web client发送消息的。

## In a Nutshell: HTTP Long Polling

To overcome this deficiency, Web app developers can implement a technique called **HTTP long polling**, where the client polls the server requesting new information. The server holds the request open until new data is available. Once available, the server responds and sends the new information. When the client receives the new information, it immediately sends another request, and the operation is repeated. This effectively emulates a server push feature.

> 所谓polling，就是指client不断的获取server端的状态。  
> Polling, refers to actively sampling the status of an external device by a client program as a synchronous activity.  
> 我之前曾经接触到一种说法，Web browser访问某个网站的时候，它的本质是查看在那一时刻Web Server的状态。
