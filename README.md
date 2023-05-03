Download Link: https://assignmentchef.com/product/solved-cs2208b-assignment-5
<br>
<strong><u>QUESTION 1 (100 marks)</u></strong>

Recursion is a method where the solution to a problem depends on solutions to smaller instances of the same problem. A function is considered recursive if it calls itself.

The following function computes <em>x<sup>n</sup></em> recursively, where <em>x</em> is an integer number and <em>n</em> is a non-negative integer number.

int power(int x, unsigned int n)

{

int y;




if (n == 0)       return 1;




if (n &amp; 1)        return x * power(x, n – 1);

else

{ y = power(x, n &gt;&gt; 1);      return y * y;

}  }

Draw <strong><u>a <em>detailed flowchart</em></u> </strong>and write an ARM assembly <strong><em><u>program</u></em></strong> to calculate <em>x<sup>n</sup></em> <strong><em><u>using the above recursive function</u></em></strong>, where <em>n</em> is passed-by-value through the stack to the function and the returned value is stored in the stack just above the parameter. <u>No other registers may be modified by the </u><u>power</u><u> function. </u>Once the control is <em><u>completely</u></em> returned back from the function (i.e., after calculating <em>x<sup>n</sup></em>), the returned value must be stored in a local variable (called <em>result</em>) in the main function. <strong><em>Your code should be highly optimized, i.e., use as little number of instructions as possible.</em></strong>

You should utilize a big enough stack so that you can calculate <em>x<sup>n</sup></em> for various <em>n</em> values.

How many stack frames are needed to calculate <em>x<sup>n</sup></em>, when <em>n</em> = 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, and 12?


