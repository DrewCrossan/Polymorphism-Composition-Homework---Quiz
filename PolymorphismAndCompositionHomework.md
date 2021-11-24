# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

Having multiple forms

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

We can have an abstract class Vehicle and 2 sub classes called Car and Bus. A Car is a Vehicle and a Bus is also a Vehicle.
Method overloading is also a form of polymorphism where you can reuse the same method name multiple times in the same class as long as the parameters are different. 

3. What can we use to implement polymorphism in Java?

We can use abstract classes or interfaces.

4. How many 'forms' can an object take when using polymorphism?

Many

5. Give an example of when you could use polymorphism.

When you want to create multiple classes that inherit the same method or parameters. E.g. if we have a class Animal with a method Sound(), we could pass that method down to child classes so that a dog.Sound() == "bark" or car.Sound() == "meow" etc.



# Composition and Aggregation

6. What do we mean by 'composition' in reference to object-oriented programming?

a class that references one or more objects of other classes in instance variables. This allows you to model a has-a association between objects. 

7. When would you use composition? Provide a simple example in Java.

When a classes is composed of another class. e.g.class Person has-a class Job. 

8. Give a difference between composition and aggregation?

Composition is a has-a relationship. Aggregation is more uses-a relationship. Composition implys ownership where as aggregation does not imply ownership. E.g. composition == a Person has-a Car. aggregation == a Person uses-a Bus.

9. What is/are the advantage(s) of using composition/aggregation?

You use fewer classes due only needing classes that you type rather than potentially inheriting useless classes/methods. Makes code DRY'er and quicker when it comes to testing. More flexible than inheritance - you can change implementation of class at run-time by changing included object, thus changing behavior of it, but you can't do this with inheritance, you can't change behavior of base class at run-time. Inheritance breaks encapsulation.

10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?

They do not exist independantly so they will need destroyed as well or will get an error.

11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?

They exist independantly, bond is weak so more flexible meaning code will be fine.