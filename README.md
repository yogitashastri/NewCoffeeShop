Problem statement :

Design and implement a coffee shop.The coffee shop should have a fixed menu.Anything ordered outside the menu should be 
rejected. Also ,there should be a fixed list of toppings available for the coffee.When the coffee is ordered it should 
list down all the details of the coffee including the toppings if any.There should be a way to introduce new products 
to the coffee shop.

Assumptions :

Application Name : NewCoffeeShop

* DarkRoast , Decaf , Expresso , and HouseBlend are diffrent types of coffee's that are available in coffee shop.
 
*French_Venilla and Chocolate are the two fixed toppings.

*French_Venilla topping is available only for cooffee of type DarkRoast.

*Chocolate topping is available only for coffee of type HouseBlend.

PsuedoCode :

1) Create an abstract parent class named Coffee.declare two instance variable. one is numOfCups.this is to take the number 
   of cups of coffe that is required by customer/user. another instance variable is description.and write getter method
   (getDescription()) for this variable.Declare one abstract method named cost(cost()).
   
2) Create child class of abstract Coffee class(parent) with name DarkRoast(Inheritance).Since DarkRoast has a topping called 
   frenchVenilla.so create instance variable named frenchVenilla of type boolean.declare one constant with datatype int 
   named FRENCH_VENILLA_COST to define french venilla topping cost and initialize it with some fixed ammount like 30/Rs.
   Override cost() method of Coffee(parent) class.initialize frenchVenilla instance variable inside the constructor.and
   the inherited variable named "description" from parent class "Coffee", initialize this variable with "information on 
   toppings and cost" inside constructor of this DarkRoast class.and ,also initialize inherited instance variable named 
   numOfCups with user inputed value inside the constructor.
   
3) Create child class of abstract Coffee class(parent class) with name Decaf(Inheritance).Decaf has no toppings.override 
   cost() method.and the inherited variable named "description" from parent class "Coffee", initialize this variable with 
   "information on cost" inside constructor of this Decaf class.and ,also initialize inherited instance variable named 
   numOfCups with user inputed value(through user facing main method using scanner) inside the constructor.
   
4) Create child class of abstract Coffee class(parent class) with name Expresso(Inheritance).Expresso has no toppings.override 
   cost() method.and the inherited variable named "description" from parent class "Coffee", initialize this variable with 
   "information on cost" inside constructor of this Expresso class.and ,also initialize inherited instance variable named 
   numOfCups with user inputed value(through user facing main method using scanner) inside the constructor.
   
5) Create child class of abstract Coffee class(parent) with name HouseBlend(Inheritance).Since HouseBlend has a topping called 
   Chocolate.so create instance variable named chocolate of type boolean.declare one constant with datatype int 
   named CHOCOLATE_COST to define Chocolate topping cost and initialize it with some fixed ammount like 20/Rs.
   Override cost() method of Coffee(parent) class.initialize chocolate instance variable inside the constructor.and
   the inherited variable named "description" from parent class "Coffee", initialize this variable with "information on 
   toppings and cost" inside constructor of this DarkRoast class.and ,also initialize inherited instance variable named 
   numOfCups with user inputed value inside the constructor.
   
6) Create a class (that exposes Menu to the user that has user facing main() method)  with name CoffeMenu.Use Scanner class
   to take user inputs.wrap entire code within main method inside try-catch blocks.using while loop display menu to the user
   to select type of Coffee that he want.when he selects his choice, it will list down all the details of the coffee like 
   information about cost and toppings.
   
Execution : 
   
   IDE Used : Eclipse
   
   Application Name : NewCoffeeShop
   
   Right_Click on Project Name => Run As => Java Application
