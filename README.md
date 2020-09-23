# ECE444-F2020-Lab2
# Sophia Ryoo
# this repo is a clone of https://github.com/miguelgrinberg/flasky

##Activity 1 (Download Flask):

![Exercise 1](https://raw.githubusercontent.com/honeyjoo/ECE444-F2020-Lab2/master/Activity%201.png "Exercise 1")

##Activity 2 (Exercise 2.2):
![Exercise 2](https://raw.githubusercontent.com/honeyjoo/ECE444-F2020-Lab2/master/Activity%202.png "Exercise 2")

##Activity 3:

Flask context globals are contexts that Flask uses to temporarily allow certain objects to be accessed globally, like global variables. Flask has two contexts: the application context and the request context. Flask activates the application and request contexts before sending a request. These contexts get removed when the request is handled so that the requests are not accessed and are only accessible when the application is active and a request is being handled. When the application context is activated, the current_app(the application instance for active application) and g(a variable that is reset for every request; application can use this variable for temporary storage while handing a request) variables become available to the thread. When the request context is activated, request and session variables become availabe. Request variable is an object that has the contents of a HTTP request sent by the client. Session is the user session, which is a dictionary that the appplication uses to store values that are remembered during requests. If any of these 4 (current_app, g, request, session) variables are accessed without an active application or request context, an error pops up.
