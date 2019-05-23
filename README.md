# NaiveTicket

The second Objects lab, from the BlueJ book's second chapter.

Look for the [Chapter 2 file](./doc/BlueJ-objects-first-ch2.pdf) you need in the [doc](./doc) folder.
There is 35 pages of reading and exercises in the chapter.

Work through all these exercises. You edit this file with your answers for these exercises.

### Exercise 2.1
* Create a TicketMachine object on the object bench.
* Upon viewing its methods, `getBalance`, `getPrice`, `insertMoney`, `printTicket`.
* Use `getPrice` method to view the value of the price of the tickets that was set when this object was created.
* Use `insertMoney` method to simulate inserting an amount of money into the machine.
* Use `getBalance` to check that the machine has a record of the amount inserted.
	* You can insert several separate amounts of money into the machine, just like you might insert multiple coins or notes into a real machine. Try inserting the exact amount required for a ticket. As this is a simple machine, a ticket will not be issued automatically, so once you have inserted enough money, call the `printTicket` method. A facsimile ticket should be printed in the BlueJ terminal window.

### Exercise 2.2
* What value is returned if you check the machine’s balance after it has printed a ticket?
Same as the price of the ticket. Nothing changes. 

### Exercise 2.3
* Experiment with inserting different amounts of money before printing tickets.
	* Do you notice anything strange about the machine’s behavior? 
	Nothing changes.
	* What happens if you insert too much money into the machine – do you receive any refund? 
	It doesn't change anything.
	* What happens if you do not insert enough and then try to print a ticket? 
	It still doesn't change anything



### Exercise 2.4
* Try to obtain a good understanding of a ticket machine’s behavior by interacting with it on the object bench before we start looking at how the `TicketMachine` class is implemented in the next section.


### Exercise 2.5
* Create another ticket machine for tickets of a different price.
	* Buy a ticket from that machine.
	* Does the printed ticket look different? 
	The price is different because we put a different value but nothing really changes when the tickets is printer.


### Exercise 2.6
* Write out what you think the outer wrappers of the `Student` and `LabClass` classes might look like – do not worry about the inner part. 
public class Student
{ 
	Inner part
			}
public class LabClass
{	
	Inner part
			}

### Exercise 2.7
Does it matter whether we write<br>
`public class TicketMachine`<br>
or<br>
`class public TicketMachine`<br>
in the outer wrapper of a class? Yes it does matter because the public class has to go first to declare a class like that.

* Edit the source of the `TicketMachine` class to make the change and then close the editor window.
	* Do you notice a change in the class diagram?: You get the red lines on the ticket machine.
	* What error message do you get when you now press the compile button? Identifier expected. 
	* Do you think this message clearly explains what is wrong? Yeah it does explain what is wrong because public is the identifier.

### Exercise 2.8
* Check whether or not it is possible to leave out the word `public` from the outer wrapper of the `TicketMachine` class. yes, It is possible. 

### Exercise 2.9
* From your earlier experimentation with the ticket machine objects within BlueJ you can probably remember the names of some of the methods – `printTicket`, for instance.
	* Look at the class definition in Code 2.1 and use this knowledge, along with the additional information about ordering we have given you, to try to make a list of the names of the fields, constructors, and methods in the `TicketMachine` class.
Fields are "price", "balance", and "total." 
Constructer: ticketCost
Methods are getprice(), getBalance(), insertMoney(), 
	* Hint: There is only one constructor in the class.

### Exercise 2.10
* Do you notice any features of the constructor that make it significantly different from the other methods of the class? No I don't think see any difference. 

### Exercise 2.11
* What do you think is the type of each of the following fields?

```java
private int count;
Its a type of integer.
private Student representative;
This is a string
private Server host;
This is a string too. 
```

### Exercise 2.12
* What are the names of the following fields?

```java
private boolean alive;
This is named alive.
private Person tutor;
This is named tutor.
private Game game;
This is named game. 
```
### Exercise 2.13

In the following field declaration from the TicketMachine class<br>

```java
private int price;
```
does it matter which order the three words appear in?
yes it does matter. You can't move around or it will give you a red lines on compiler. 

* Edit the `TicketMachine` class to try different orderings. After each change, close the editor.
	* Does the appearance of the class diagram after each change give you a clue as to whether or not other orderings are possible? Well it does matter if you move the words around. 
	* Check by pressing the compile button to see if there is an error message.
	<Identifier> expected
	* Make sure that you reinstantiate the original version after your experiments!

### Exercise 2.14
* Is it always necessary to have a semicolon at the end of a field declaration?
Yes, it signifies that the declaration is over.
* Once again, experiment via the editor. 
* The rule you will learn here is an important one, so be sure to remember it.


### Exercise 2.15
* Write in full the declaration for a field of type `int` whose name is `status`.
Private int status

### Exercise 2.16
* To what class does the following constructor belong?
```
public Student(String name)
```
Student class. 

### Exercise 2.17
* How many parameters does the following constructor have and what are their types?
There are 2 types of constructor. 1 is string and other one is double type. 
```
public Book(String title, double price)
```

### Exercise 2.18
* Can you guess what types some of the `Book` class’s fields might be? It would be a string type.
* Can you assume anything about the names of its fields? It could have a integer or you could have a double. 

Work all Exercises from 2.19 to 2.58 that are **NOT** marked *Challenge exercise*.
READ upto and INCLUDING section 2.15 of this chapter.


2.19: public pet (String petsName)
	{
		name = petsName;
	}

2.21  Get price method comes out as what the price was initiated for the ticket but getBalance still returns as money that was paid for the ticket.

2.22 I get the price on how much I have paid in the machine. 

2.23 No it doesn't change anything.

2.24 Public int getTotal()
	{ 
		return total

	}

2.25 missing return statement 

2.26 The difference between getPrice and printTicket is getPrice returns the price and printTicket prints you the tickets of how much you have paid in the machine. 

2.27 No they don't because they don't have a return method and has the void as a header. 

2.29 because of the public void in the header. 

2.30 public void setPrice(int ticketCost)
	{
		price = ticketCost + price;
	}

2.31 public void increase(int points)
	{
	score = score + points;
	}

2.32 public void increase(int amount)
	{
	price = price - amount;
	}
2.33 Done on BlueJ 

2.34 Done on BlueJ

2.35 It did show different amounts because it was sold for different price or entered different price. 

2.36 It would print out ("# " + "price" + " cents.") 

2.37 It would print out ("# price cents.")

2.38 no because its a string. Its not a variable anymore. 

2.39 It fixes the price at 1000 cents. 

2.40 Its a mutator. 

2.41 It is a mutator. 

2.42 
2.43

2.44 It doesn't let me insert a value greater than or equal to Zero. 

2.45 yes, it did have two different values. 

2.46 When you pay for the ticket, it removes the price from the balance. When you put money inside the ticket, it adds the total. 

2.47 No it doesn't let me pay because its impossible to add a negative value. 

2.48 1: Multiplication *
2: Division / 
3: Modulus %

2.49 public store()
	{
	savings = price * discount;
	}

2.50  public Mean
	{mean = total/count;
	}
2.51 public void anything()
	{
	if (price > budget)
	System.out.println("Too Expensive");
	else return
	system.out.println("Just Right");
	}
2.52 Public void anything()
	{
	if (price>budget)
	system.out.println("Too expensive, current budget:" + budget);
	else return system.out.println("Just Right");
	}


2.54 it doesn't compile because the method does not make sure. It doesn't have an end. 

2.55 public int emptyMachine()
	{
	total = 0;
	return total;
	}

2.56 It is a mutator 














































