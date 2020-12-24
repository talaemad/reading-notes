# comparison operators: evaluating conditions

* you can evaluate a situation by comparing one value in the script to what you expect it might be, The result will be a bool, : true or false.

**==** =>equal to, compare the value not data type.
**===** => strict equal to, compare the value and the data type.
**!=** => not equal, compare the value not data type.
**!==** => strict not equal to, compare the value and the data type.
**>**  => is greater than, check the left number is greater than the right number. 
**>=** => greater than or equal to, check the left number is greater or equal to the right number.
**<**less than, check the left number is less the right number. 
**<=** less than or equal to, check the left number is less or equal to the right number.

# logical operators

* usually return single values of true or false.
* logical operators allow you to compare the results of more than one comparison operator.
**&&** => logical and, test more than one condition, return true when both expressions true.
**||** => logical or, test at least one condition, return true always except when both false return false.
**!** => logical not, takes a single boolean value and inverts it.

# Loops 

* loops check a condition. if it returns true, a code block will run. then the condition will be checked again and if it still returns true, the code block will run again. it repeats until it becomes false.

* loop types:
**For** => use it if you know how much time you need to run the code.
**While** => use it if you don't how many times the code needs to run.
**Do While** => it will always run time, even if the condition is false from the beginning.

* For loop: use counter as condution.(initialization `var i=0 `,condition `i<value` ,update`i++`)
* in every loop it need to check the condition and update the value. it will end looping when condition return false.

* while loop: This loop will continue to run for as long as the condition in the parentheses is true.