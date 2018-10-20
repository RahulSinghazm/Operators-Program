# Operators

## What are operators in python?
Operators are special symbols in Python that carry out arithmetic or logical computation. 
The value that the operator operates on is called the operand.

### For example:
<pre>
>>> 2+3
5
</pre>

Here, + is the operator that performs addition. 2 and 3 are the operands and 5
is the output of the operation.

## Arithmetic operators:
Arithmetic operators are used to perform mathematical operations like addition, 
subtraction, multiplication etc.

<center>## Arithmetic operators in Python:</center>
<pre>
Operator        	Meaning                                                                 	Example
</pre><pre>
+                 Add two operands or unary plus	x + y                                      +2

-	              Subtract right operand from the left or unary minus	x - y                  -2

*                 Multiply two operands                                                      x * y
    
/	              Divide left operand by the right one (always results into float)	         x / y

%	              Modulus - remainder of the division of left operand by the right	         x % y 
                                                                                             (remainder of x/y)
                                                                                             
//	              Floor division - division that results into whole number adjusted          x // y
                  to the left in the number line	
                  
**	              Exponent - left operand raised to the power of right	                      x**y (x to the power y)
</pre>

### Example #1: Arithmetic operators in Python:

<pre>x = 15
y = 4

# Output: x + y = 19
print('x + y =',x+y)

# Output: x - y = 11
print('x - y =',x-y)

# Output: x * y = 60
print('x * y =',x*y)

# Output: x / y = 3.75
print('x / y =',x/y)

# Output: x // y = 3
print('x // y =',x//y)

# Output: x ** y = 50625
print('x ** y =',x**y)
</pre>

### Output:
* When you run the program, the output will be:
<pre>
x + y = 19
x - y = 11
x * y = 60
x / y = 3.75
x // y = 3
x ** y = 50625
</pre>

## Comparison operators:
Comparison operators are used to compare values. It either returns True or False according 
to the condition.

<center>## Comparision operators in Python:</center>
<pre>
Operator  Meaning	                                                               Example
</pre>
<pre>
>	       Greater that - True if left operand is greater than the right	       x > y

<	       Less that - True if left operand is less than the right	               x < y

==	       Equal to - True if both operands are equal	                           x == y

!=	       Not equal to - True if operands are not equal	                       x != y

>=	       Greater than or equal to - True if left operand is greater than         x >= y
           or equal to the right	
           
<=	       Less than or equal to - True if left operand is less than or equal      x <= y
           to the right	
</pre>

### Example #2: Comparison operators in Python:

<pre>
x = 10
y = 12

# Output: x > y is False
print('x > y  is',x>y)

# Output: x < y is True
print('x < y  is',x<y)

# Output: x == y is False
print('x == y is',x==y)

# Output: x != y is True
print('x != y is',x!=y)

# Output: x >= y is False
print('x >= y is',x>=y)

# Output: x <= y is True
print('x <= y is',x<=y)
</pre>

### Output:
<pre>
('x > y  is', False)
('x < y  is', True)
('x == y is', False)
('x != y is', True)
('x >= y is', False)
('x <= y is', True)
</pre>

## Logical operators:
Logical operators are the and, or, not operators.

<center>### Logical operators in Python</center>

<pre>
Operator	Meaning	                                            Example
</pre>
<pre>
and	        True if both the operands are true	                x and y

or	        True if either of the operands is true	            x or y

not	        True if operand is false (complements the operand)	not x
</pre>

### Example #3: Logical Operators in Python:

<pre>
x = True
y = False

# Output: x and y is False
print('x and y is',x and y)

# Output: x or y is True
print('x or y is',x or y)

# Output: not x is False
print('not x is',not x)
</pre>

### Output:
<pre>
x and y is False
x or y is True
not x is False
</pre>

## Bitwise operators:

Bitwise operators act on operands as if they were string of binary digits.
It operates bit by bit, hence the name.

For example, 2 is 10 in binary and 7 is 111.

In the table below: Let x = 10 (0000 1010 in binary) and y = 4 (0000 0100 in binary)

<center>### Bitwise operators in Python</center>

<pre>
Operator	  Meaning	                Example
</pre>
<pre>
&	          Bitwise AND	            x& y = 0 (0000 0000)

|	          Bitwise OR	            x | y = 14 (0000 1110)

~	          Bitwise NOT       	    ~x = -11 (1111 0101)

^	          Bitwise XOR	            x ^ y = 14 (0000 1110)

>>	          Bitwise right shift	    x>> 2 = 2 (0000 0010)

<<	          Bitwise left shift	    x<< 2 = 40 (0010 1000)
</pre>

## Assignment operators:
Assignment operators are used in Python to assign values to variables.

a = 5 is a simple assignment operator that assigns the value 5 on the right to the variable a on the left.

There are various compound operators in Python like a += 5 that adds to the variable and later assigns the same. 
It is equivalent to a = a + 5.

<center>### Assignment operators in Python</center>

<pre>
Operator	      Example	                Equivatent to
</pre>
<pre>
=	            x = 5	                x = 5

+=	            x += 5	                x = x + 5

-=	            x -= 5	                x = x - 5

*=	            x *= 5	                x = x * 5

/=	            x /= 5	                x = x / 5

%=	            x %= 5	                x = x % 5

//=	            x //= 5	                x = x // 5

**=	            x **= 5	                x = x ** 5

&=	            x &= 5	                x = x & 5

|=	            x |= 5	                x = x | 5

^=	            x ^= 5	                x = x ^ 5

>>=	            x >>= 5	                x = x >> 5

<<=	            x <<= 5	                x = x << 5
</pre>


## Special operators:
Python language offers some special type of operators like the identity operator or the membership operator. 
They are described below with examples.

### Identity operators:
is and is not are the identity operators in Python. They are used to check if two values (or variables) are 
located on the same part of the memory. Two variables that are equal does not imply that they are identical.

<center>###Identity operators in Python</center>

<pre>
Operator	  Meaning	                                                                 Example
</pre>
<pre>
is	          True if the operands are identical (refer to the same object)	              x is True

is not	      True if the operands are not identical (do not refer to the same object)	  x is not True
</pre>

### Example #4: Identity operators in Python:
<pre>
x1 = 5
y1 = 5
x2 = 'Hello'
y2 = 'Hello'
x3 = [1,2,3]
y3 = [1,2,3]

# Output: False
print(x1 is not y1)

# Output: True
print(x2 is y2)

# Output: False
print(x3 is y3)
</pre>

### Output:
<pre>
False
True
False
</pre>

Here, we see that x1 and y1 are integers of same values, so they are equal as well as identical. 
Same is the case with x2 and y2 (strings).

But x3 and y3 are list. They are equal but not identical. It is because interpreter locates them 
separately in memory although they are equal.

## Membership operators:
in and not in are the membership operators in Python. They are used to test whether a value or 
variable is found in a sequence (string, list, tuple, set and dictionary).

In a dictionary we can only test for presence of key, not the value.

<pre>
Operator	      Meaning	                                                Example
</pre>
<pre>
in	            True if value/variable is found in the sequence	        5 in x

not in	        True if value/variable is not found in the sequence	    5 not in x
</pre>

### Example #5: Membership operators in Python:

<pre>
x = 'Hello world'
y = {1:'a',2:'b'}

# Output: True
print('H' in x)

# Output: True
print('hello' not in x)

# Output: True
print(1 in y)

# Output: False
print('a' in y)
</pre>

### Output:
<pre>
True
True
True
False
</pre>

Here, 'H' is in x but 'hello' is not present in x (remember, Python is case sensitive). 
Similary, 1 is key and 'a' is the value in dictionary y. Hence, 'a' in y returns False.
