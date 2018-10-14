# PHP

The PHP code is written inside an HTML file using the tags "\<?php      ?>".
where starting tag is "\<?php" and the ending tag is "?\>".

* The code isn't going show if the user tries to view source.

* Every php statement should end with a semi colon.

 ## Comment types

  1. Single Line: use // This is a single comment,    or #This is also a single line comment.

  2. Multiple Line: use  /*                      This is 

     a multiline

     Comment                                 */.

   ## Output Statement

​	**Echo**: It outputs whatever is written after it. eg:.

*  echo thisWillBeTheOutput;        **Output**: thisWillBeTheOutput

* echo "this\\"WillBeALittle\"Different";   **Output**: this"WillBeALittle"Different

 as shown above double quotes allows you to use the *escape sequences*. 

* Do not use single quotes they ignore the escape sequences.

* You can also not print out variables directly inside using quotes.

 ## Variables

​	They begin with  **$** sign. eg.: $variableName ;

​	$userName = $_POST['username'];

as HTML uses 'post way of passing information' (currently so not know what that means) therefore $_POST[' '] thing is used.			(not sure about this one)
here userName is the userName that is defined in the HTML file. By this statement the userName variable gets the value of userName in the HTML .

* First digit of the variable defined should be an alphabet after that anything will do.

* Variable Names are case sensitive.

* Whenever a variable is created, it is automatically given a Data type depending upon the value it is given.

* Data type can be of: Integer, Float, String, Boolean, Array, Object.

* By default a variable will get the value of Null.

* String concatenation can be done using **"."** operator.

  ~~~php
  echo $userName . "</br>";
  echo $streetAddress . "</br>";
  echo $cityAddress . "</br>";
  /* Output:
  username
  streetaddress
  cityaddress
  */
  ~~~

  ### Multiple Line Strings

  ~~~php
  //define here whatever you want not to go in the string.(didn't really know what that mean now).
  $str = <<<EOD
  The cudtomers name is 
  $userName and they
  live at $streetAddress
  in $cityAddress</br>
  EOD;
  echo $str;
  /*	Output:
  	The customers name is Derek and they live at 123 Main St in Derry
  */
  ~~~

  ### Constants

  ~~~php 
  define('PI' , 3.14159);
  echo "The value of PI is " , PI;
  // You would want to use UPPERCASE in the condtants, that's what he said in the video
  /*	Output:
  	The value of PI is 3.14159
  */
  ~~~

  ### Basic Arithmetic

  ~~~php
  echo "</br> 5 + 2 = " . (5+2);
  echo "</br> 5 - 2 = " . (5-2);
  echo "</br> 5 * 2 = " . (5*2);
  echo "</br> 5 / 2 = " . (dataType) (5/2); //dataType is the required data type in which you want to get the output of (5/2)
  echo "</br> 5 % 2 = " . (5%2) . "</br>";
  /*
  	Output:
  		5 + 2 = 7
  		5 - 2 = 3
  		5 * 2 = 10
  		5 / 2 = 2	// if dataType is integer
  		5 % 2 = 1
  */
  ~~~

  #### Shortcuts

  ~~~php
  $randNum = 5;
  echo $randNum += 10 . "</br>";
  echo $randNum -= 10 . "</br>";
  echo $randNum *= 10 . "</br>";
  echo $randNum /= 10 . "</br>";
  echo $randNum %= 10 . "</br>";
  /*
  	Output:
  		15 			// 5 + 10
  		-5			// 5 - 10
  		50			// 5 * 10
  		0.5			// 5 / 10
  		0			// 5 % 10
  */
  //Here randNum is asigned a new value in every statement.
  ~~~

  ### Incrementing

  ~~~php
  
  ~~~


