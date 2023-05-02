Download Link: https://assignmentchef.com/product/solved-cmsc203-assignment-6-bradley-beverage-shop-2
<br>
Bradley Beverage Shop

Bradley shop is a family owned store that sells beverages.  The store offers 3 types of beverages: Coffee, Alcohol, and Smoothie. The store is open from 8 in the morning to 11 pm in the afternoon.  The owner of the shop likes to automate the order transactions and reports and purchase a software for testing order activities for one month. You are asked to implement this software based on the following requirements.

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Assignment Description</strong></td>

  </tr>

 </tbody>

</table>




BevShop (The Data Manager Class)




The BevShop offers 3 types of beverages: Coffee, Alcoholic and Smoothie. Beverages can be ordered in 3 different sizes: Small, medium and large. All the beverage types have a base price. In addition there are additional charges depending on the size and specific add-ons for each type of beverage.




The BevShop has the following functionality:

<ul>

 <li>Create and process orders of different types of beverages</li>

 <li>Provide information on all the orders</li>

 <li>Total amount on a specific order</li>

 <li>Monthly total number of orders</li>

 <li>Monthly sale report</li>

</ul>

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Concepts tested by this assignment</strong></td>

  </tr>

 </tbody>

</table>













<ul>

 <li>Aggregation</li>

 <li>Searching an Arraylist</li>

 <li>Selection sort</li>

 <li>Enumeration</li>

 <li>Inheritance</li>

 <li>Interface</li>

 <li>Polymorphism</li>

 <li>Abstract classes</li>

 <li>Overriding methods</li>

 <li></li>

</ul>













<table width="100%">

 <tbody>

  <tr>

   <td><strong>Interfaces</strong></td>

  </tr>

 </tbody>

</table>







<strong>OrderInterface </strong>

This interface is provided for you and is implemented by the <strong>Order</strong> class.




<strong>BevShopInterface</strong>

This interface is provided for you and is implemented by the <strong>BevShop</strong> class.
















<table width="100%">

 <tbody>

  <tr>

   <td><strong>Classes</strong></td>

  </tr>

 </tbody>

</table>







<strong>Enumerated Type – DAY</strong>

Create an enumerated type called <strong>DAY</strong>.  The valid values will be MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY, SUNDAY.

<strong>Enumerated Type – SIZE</strong>

Create an enumerated type called <strong>SIZE</strong>.  The valid values will be SMALL, MEDIUM, LARGE.

<strong>Enumerated Type – TYPE</strong>

Create an enumerated type called <strong>TYPE</strong>.  The valid values will be COFFEE, SMOOTHIE, ALCOHOL

<strong> </strong>

<strong>Data Element – Beverage</strong>

Create an abstract class called <strong>Beverage</strong> with:

<ul>

 <li>Instance variables for beverage name, beverage type, size, and constant attributes for the base price ($2.0) and size price (additional $1 to go a size up).</li>

 <li>A parametrized constructor to create a Beverage object given its name, type and size</li>

 <li>An abstract methods called <strong>calcPrice </strong>that calculates and returns the beverage price<strong>.</strong></li>

 <li>An Overridden<strong> toString</strong> method: String representation for Beverage including the name and size</li>

 <li>An Overridden<strong> equals</strong> method: checks equality based on name, type, size of the beverage</li>

 <li>getters and setters and any other methods that are needed for your design.</li>

 <li>Use finals to represent constants.</li>

</ul>







<strong>Data Element – subclasses of Beverage</strong>

Create the following subclasses of Beverage for the 3 types of beverages:




<strong><u>Coffee</u></strong>

<ul>

 <li>Contains additional instance variables of type boolean to indicate if it contains extra shot of coffee (additional cost of 50 cents) and extra syrup (additional cost of 50 cents).</li>

 <li>A parametrized constructor</li>

 <li>An Overridden<strong> toString</strong> method: String representation of Coffee beverage, including the name , size ,  whether it contains extra shot, extra syrup and the price of the coffee</li>

 <li>An Overridden<strong> calcPrice</strong></li>

 <li>An Overridden<strong> equals</strong> method: checks equality based on the Beverage class <strong>equals</strong> method and additional instance variables for this class.</li>

 <li>getters and setters and any other methods that are needed for your design.</li>

 <li>Use finals to represent constants.</li>

</ul>

<strong><u>Smoothie</u></strong>

<ul>

 <li>Contains additional instance variables for number of fruits and boolean variable to indicate if protein powder is added to the beverage. The cost of adding protein is $1.50 and each additional fruit costs 50 cents.</li>

 <li>A parametrized constructor</li>

 <li>An Overridden<strong> toString</strong> method: String representation of a Smoothie drink including the name , size, whether or not protein is added , number of fruits and the price</li>

 <li>An Overridden<strong> equals</strong> method: checks equality based on the Beverage class <strong>equals</strong> method and additional instance variables for this class.</li>

 <li>An Overridden<strong> calcPrice</strong></li>

 <li>getters and setters and any other methods that are needed for your design.</li>

 <li>Use finals to represent constants.</li>

</ul>

<strong> </strong>

<strong><u>Alcohol</u></strong>

<ul>

 <li>Contains additional instance variable for weather or not it is offered in the weekend. The additional cost for drinks offered in the weekend is 60 cents.</li>

 <li>A parametrized constructor</li>

 <li>An Overridden<strong> toString</strong> method: String representation of a alcohol drink including the name, size, whether or not beverage is offered in the weekend and the price.</li>

 <li>An Overridden<strong> equals</strong> method: checks equality based on the Beverage class <strong>equals</strong> method and additional instance variables for this class.</li>

 <li>An Overridden<strong> calcPrice</strong></li>

 <li>getters and setters and any other methods that are needed for your design.</li>

 <li>Use finals to represent constants.</li>

</ul>




<strong>Data Element – Customer</strong>

Create a class to represent a customer.

<ul>

 <li>Instance variables for name and age</li>

 <li>A parametrized constructor</li>

 <li>A Copy constructor</li>

 <li>An Overridden<strong> toString</strong> method: String representation for Customer including the name and age</li>

 <li>getters and setters and any other methods that are needed for your design.</li>

</ul>




<strong>Data Element – Order </strong>

Create a class to represent an order. This class implements two interfaces: <strong>OrderInterface</strong> and <strong>Comparable.  </strong>

<ul>

 <li>Instance variables for order number, order time, order day and customer and a list of beverages within this order</li>

 <li>A method to generate a random number within the range of 10000 and 90000</li>

 <li>A parametrized constructor</li>

 <li>A method called <strong>addNewBeverage</strong> that adds a beverage to the order. This is an overloaded method to add different beverages to the order.  Refer to the interface OrderInterface provided for you,</li>

 <li>An Overridden<strong> toString</strong> method: Includes order number, time, day, customer name , customer age and the list of beverages (with information of the beverage).</li>

 <li>Override the <strong>compareTo</strong> method to compare this order with another order based on the order number. Returns 0 if this order number is same as another order’s order number, 1 if it is greater than another order’s order number, -1 if it smaller than another order’s order number.</li>

 <li>getters and setters and any other methods that are needed for your design.   <strong>Note: The getter method for the customer returns a Deep copy of the customer.</strong></li>

 <li>Refer to provided <strong>OrderInterface</strong> interface for additional methods.</li>

 <li></li>

</ul>




<strong>Data Manager – BevShop</strong>

Create a class to represent a beverage shop. This class implements <strong>BevShopInterface</strong> provided to you.

<ul>

 <li>Instance variable for the number of Alcohol drinks ordered for the <strong><u>current order</u></strong>. The current order in process can have at most <strong>3</strong> alcoholic beverages.</li>

 <li>An instance list to keep track of orders</li>

 <li>The minimum age to order alcohol drink is 21</li>

 <li>time, order day and customer and a list of beverages <strong>Order </strong>within this order</li>

 <li>An Overridden<strong> toString</strong> method: The string representation of all the orders and the total monthly sale.</li>

 <li>Refer to provided <strong>BevShopInterface</strong> interface for additional methods.</li>

</ul>




<strong>Data Structure</strong>

<ul>

 <li>You will be using an Arraylist within your Order to hold beverages of the order and BevShop class to hold orders.</li>

</ul>

<strong>External Documentation</strong>

<ul>

 <li>Provide a UML diagram with all classes and their relationships.</li>

</ul>






































































<strong>Testing</strong>

There is no GUI provided for this project. To test your project you may (recommended but not required) to create your own driver file for each class as you gradually implement code.

<ul>

 <li>Ensure that java produces the following output:</li>

</ul>






































































<ul>

 <li>Ensure that all the given JUnit tests .java succeed.</li>

</ul>


































<strong><u> </u></strong>

<strong><u> </u></strong>

<strong><u> </u></strong>

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Deliverables</strong></td>

  </tr>

 </tbody>

</table>

<strong><u>Deliverables / Submissions</u>: </strong>

<strong> </strong>

GitHub: Upload all input files and all implemented files into GitHub in the repo you created in Lab 1 in a directory named CMSC203_Assignment6.

<strong><u> </u></strong>

Design: UML class diagram.

Implementation: Submit a compressed file containing the follow (see below):  The Java application (it must compile and run correctly); a write-up as specified below.  Be sure to review the provided project rubric to understand project expectations.  The write-up will include:

<ul>

 <li>UML diagram – latest version</li>

</ul>

<ul>

 <li>Any assumptions that you are making for this project</li>

 <li>Highlights of your learning experience. What were you successful at, and what (if anything) were you not able to implement?</li>

</ul>




<strong><u>Deliverable format</u>:</strong> The above deliverables will be packaged as follows. Two compressed files in the following formats:

<strong><u>Notice:</u></strong> Only submit the files that you implemented/Modified.

<ul>

 <li>zip, a compressed file in the zip format, with the following:

  <ul>

   <li>Write up (Word document) – reflection paragraphs</li>

   <li>UML Diagram – latest version (Word or jpg document)</li>

  </ul></li>

</ul>

<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     <li style="list-style-type: none;">

      <ul>

       <li>subdirectories and other files</li>

       <li>File1.html (example)</li>

       <li>File2.html (example)</li>

      </ul></li>

    </ul></li>

  </ul></li>

</ul>

<ul>

 <li>src (directory) – Java and JUnit tests files</li>

</ul>

<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     <li style="list-style-type: none;">

      <ul>

       <li>File1.java (example)</li>

       <li>File2.java (example)</li>

       <li>Filetest.java (example)</li>

      </ul></li>

    </ul></li>

  </ul></li>

</ul>

<ul>

 <li>zip, a compressed file containing one or more Java files:

  <ul>

   <li>java (example)</li>

   <li>java (example)</li>

   <li>java (example)</li>

  </ul></li>

</ul>

This folder should contain Java source files only








