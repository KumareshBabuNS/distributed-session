# distributed-session

This is a sample application for distributed http session that managed by redis by using spring session.
Install redis with version above 2.8+ first.

To test the application, start the application twice with different port number. 

Call http://localhost:8080/doLogin and then call http://localhost:8080/main, pay attention on the cookie session id.
rerun above step in a different server like 8081, and also take a look at the session id. 

They should use the same session id since it is now managed by redis and shared among services.
