# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.

# Decorator pattern -

# Summary:
    Decorator pattern is used for extension at runtime and to avoid overuse of inheritance

# what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example

    Give additional responsibilities to an object with less effort (without any code changes)

    Example:

    Consider a gift shop and you would like to buy a gift and if you would like to add a gift wrap to the item, bow tie, sticker,
    attach a greeting card, a message, a rose etc.

    The requirements for each customer may vary, a customer may buy a gift without wrapping it also.
    The wrappers are added at runtime as each customer's wish. This is when decorator pattern is used.

# Basic idea of the pattern:
    Add additional responsibilities to an object at runtime.

# Advantage:

    Decorators can be used to get different combinations at runtime.

# Disadvantage:

    If there are only few decorator to be used, the pattern can be an over engineered solution.


# Adapter pattern -

# Summary:
   Adapter pattern is used when two incompatible objects want to communicate with each other. Adapter class is actually a wrapper class.

# What kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example

    When there are two independent objects and they are incompatible, Adapter pattern can be used to act as a bridge for communication.

    Example:

    There is a BoschEmployee class and TCQClass class. Learning is an interface with learn() method.
    TCQClass implements Learning Interface.

    And a BoschEmployee wants to attend a TCQ class. We can create an adapter class BoschTCQ which extends BoschEmployee and implements
    Learning interface.

    So now BoschEmployee can also attend TCQClasses.


# Basic idea of the pattern:
    When you want a class to make use of features of the class with incompatible interface.

# Advantage:

    Reusability of existing functionality.
    You can also introduce new functionalities without tampering or doing any code changes to the existing classes.

# Disadvantage:

    Overuse of the pattern may lead to having a lot of adaptations before the desired type is reached.

# Memento pattern -

# Summary:
  Memento design pattern is used to implement the undo operation

# What kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example

    Mainly used for database transactions to preserve history and rollback on failures.

    Example:

    There is an Update class that updates value of a database. It will have Transactions class which will have data of latest transaction.

    There will be a TransactionHistory class which will keep track of the entire transaction.

    Whenever the update method is invoked, the transaction will be saved in transactionHistory, so in case of any failure, it can be reset.

# Basic idea of the pattern:
    When you want a class to keep track of all the changes, so you can implement the rollback operation.

# Advantage:

    When there is a failure, there is a need to save previous state and Memento pattern is of great help.

# Disadvantage:

    Whenever the data stored for each transaction is huge, the Memento pattern leads to high memory usage.

# Prototype pattern -

# Summary:
  Prototype pattern means copying something that already exists.
  When you want to create an object similar to another object, certain fields my be private and inaccessible. Prototype pattern 
  enables easy cloning of objects.

# What kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example

    Prototype pattern is used when object creation is costly.
    And also when you want to hide how the object is created.

    Example:

    When you want to add similar objects to different shopping carts, prototyping can be used.


# Basic idea of the pattern:
    When you want a class to keep track of all the changes, so you can implement the rollback operation.

# Advantage:

    When creation is costly, we use prototype pattern there by saving time and improving performance.


# Disadvantage:

    Whenever there is a circular reference, cloning such objects will be difficult.
