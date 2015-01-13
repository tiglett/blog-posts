# Weekly update [04/11/2013]
This week I was working on the design of the app in preparation for the Design Plan document. I have also been working on the UML class diagram for the app.

I plan on completing the class diagram in the week starting the 11th so that we can all start prototyping classes. In the class diagram there are many interfaces rather than classes. This is so that once we have decided how everything will interact and finalised the interfaces then it does not matter what changes people make to their code base – as long as their code correctly implements the interfaces methods then its usage within other classes will remain the same.

This also means that if we want to prototype a new class that implements one of these interfaces, we simply need to change the line which instantiates that variable e.g:
InterfaceY myShinyVariable = new ClassX();

 

would become:
InterfaceY myShinyVariable = new ClassX();
and would be accessed the same way.

Well, that pretty much ties up this week’s work.

Hours spent this week:

 * Internal meeting: 1 hour
 * UML class diagram: 2 hours
 * Total this week: 3 hours
 * Total so far: 10 hours
