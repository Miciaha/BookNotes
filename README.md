# Design Patterns [WIP]
This project follows the book Design Patterns by Gamma et al. 
While the examples in the book are written in C++ and Smalltalk, I thought it
would be beneficial to translate them into Java for learning purposes.

|        | Creational                                                   | Structural                                                                                       | Behavioral                                                                                                                        |
|--------|--------------------------------------------------------------|--------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| Class  | Factory Method                                               | Adapter (class)                                                                                  | Interpreter, Template Method                                                                                                      |
| Object | Abstract Factory <br/> Builder<br/> Prototype<br/> Singleton | Adapter (object)<br/> Bridge<br/> Composite<br/> Decorator<br/> Facade<br/> Flyweight<br/> Proxy | Chain of Responsibility<br/> Command<br/> Iterator<br/> Mediator<br/> Memento<br/> Observer<br/> State<br/> Strategy<br/> Visitor |

### Principles of Object-Oriented Design

*Program to an interface, not an implementation*

*Favor object composition over class inheritance*

### Common Causes of Redesign and Design Patterns for Remedy
| Cause                                                     | Issue                                                                                                  | Solution                                                                                                   | Design patterns                                                                        |
|-----------------------------------------------------------|--------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
| *Creating an object by specifying a class explicitly*     | Commits developer to a particular implementation instead of an interface                               | Create objects indirectly                                                                                  | Abstract Factory, Factory Method, Prototype                                            |
| *Dependence on specific operations*                       | Hard-coded requests commits to one way of handling a request                                           | Avoid hard-coded requests                                                                                  | Chain of Responsibility, Command                                                       |
| *Dependence on hardware and software platform*            | Creates porting difficulties                                                                           | Limit platform dependencies                                                                                | Abstract Factory, Bridge                                                               |
| *Dependence on object representations or implementations* | Clients may have meta information that would need to change as the object changes                      | Hide information from clients                                                                              | Abstract Factory, Bridge, Memento, Proxy                                               |
| *Algorithmic dependencies*                                | Algorithms are often modified and optimized which would lead to dependent objects to change as they do | Algorithms that are likely to be changed should be isolated                                                | Builder, Iterator, Strategy, Template Method, Visitor                                  |
| *Tight coupling*                                          | Hard to reuse classes in isolation. Leads to monolithic systems. Hard to learn, port, and maintain.    | Implement loose coupling                                                                                   | Abstract Factory, Bridge, Chain of Responsibility, Command, Facade, Mediator, Observer |
| *Extending functionality by subclassing*                  | Requires an in-depth understanding of the parent class and could lead to additional subclasses.        | Introduce customized functionality by defining one subclass and composing its instances with existing ones | Bridge, Chain of Responsibility, Composite, Decorator, Observer, Strategy              |
| *Inability to alter classes conveniently*                 | Modifying commercial libraries and/or complex classes with many subclasses can be difficult            | Use design patterns                                                                                        | Adapter, Decorator, Visitor                                                            |
