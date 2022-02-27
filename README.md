# Sat-Sun
Offline classes

--------------------------------------------------
-> Class is an user define data type.

Syntax:
=========
<modifier> class <name> <extends> <implements>
	{
		// body => member  either STATIC or INSTANCE
					1. variables
					2. methods
					3. constructor*
					4. initializer blocks
					5. inner/nested class
					
	}

Example:
----------
	class Car
	{
		int h;  // instance variable
		int w; 	// instance variable	
static	int wc; // static variable
		
		void move(){} // instance method		
static	void avg(){} // static method
		
	}

-----------------------------------------------------------------
*)variable is the name of memory location where data is stored.

-> static members are associated with class or class name.
-> instance members are associated with object or object reference.
------------------------------------------------------------------
Object:
----------
1. Object is an real world entity.
2. Object is an instance of a class.

Syntax:
---------
		<type>	<var> = new <type>(<parameterList>)

Example:
==========
		
		int i = 10;
		
		Car c1 = new Car();
		Car c2 = new Car();

		
Accessing Members:
----------------------		
1. <ClassName>.<member>    (only static members)
2. <ObjRef>.<member>  (instance as well as static)
3. <member>		
-------------------------------------------------
	Car.wc = 50; // OK

	 c2.w = 20;
	 c1.h =15;	
	------------------------

      Car.h =25; //error	
	  c1.wc= 100; // OK (not recommended)
		
------------------------------------------------------------------
The main():
=================

 public class Test
 {

	public static void main(String[] shad)
		{
		}
}

-> called by JVM which is an external entity, hence declared public.
-> due to static , called directly with class name, otherwise, JVM will have to create an object which is an unnecessary task.

				Test obj = new Test();
				obj.main(----);

				Test.main(-----);

------------------------------------------------------------
Ptinting in Java:
-------------------

System.out.print(data) -> data
System.out.println(data) -> data + newLine
System.out.printf(data) -> data + formatting like c/c++

  int i =10;
  
  System.out.println(i); //  10
  System.out.println('i'); // i as char value
  System.out.println("i"); // i as string value
  System.out.println(10); // 10 as number or int value
  System.out.println("10"); // 10 as a string value
  System.out.println( 2 * 5); // 10

class B
{
	void foo()
		{
		
		}
}
-----------------
B v1 = new B();
   v1.foo();
-----------------
class A
	{
		--------
		----
		static B v2;
		-------
		---
	}

 A.v2.foo();
----------------------------------------------------------------
System.out.println()

A -> System class
B -> PrintStream class

--------------------------------------------------------------
Tokens: are basic building block of a source code.
----------------------------------------------------
public class A
{
 int i = 10;
}
================================================================================

----------------Data Types------------------------

Data Types (1Byte = 8 bits) Binary Digit
-----------
1. Primitive
	|-Boolean
		|-boolean(NA)
	
	|-Numeric
		|-Integral
			|-Character
				|-char (2B)
			|-Integer
				|-byte (1B)
				|-short(2B)
				|-int (4B)
				|-long (8B)
		|-Floating Point
			|-float (4B)
			|-double (8B)


2. Reference Type
	a. class
	b. interface
	c. array
	d. enum
	d. annotation

-----------------------------------------------
byte -> short -> int -> long -> float -> double
		char -> int
		
-> Widening is done implicitly.
-> Narrowing requires casting.



================================================================================

Token 
------
 |- keywords: [are predefine words to the compiler] -> 53 (lowercase)
		*) Reserved words (goto, const)
 
 |- Indentifiers: [name of class, method, variable, etc aalled identifier]
			1. only letter, digit, '_', '$'
			2. never starts from digit
			3. cannot use keywords

 |- Literals:[values]
	    |- Integer values: {10, -10, 0b10, 010, 0x10 }
				*)default data type is int
				
        |- Floating point values {2.3, -2.3, 2E-19, 2e19}
 				*)default data type is double 
				
		|- Boolean {true, false}
		
		|- Character {'a', '1', '#'}
			|- Escape sequence
		|- String {"a","1","Shadab@gmail.com"}
 
  |- Operators
  |- White spaces(space, tab, enter)
  |- Comments
		|- // single line comments
		|- /* Multi Line comments */
		|- /** Java Documentation Comment*/

-----------------------------------------------------------
Control flow statements:
---------------------------
1) if(<boolExpr>)
	{
		//body
	}

2) if(<boolExpr>)
	{
		//body
	}
	else
	{
		//body
	}

3) if(<boolExpr>)
	{
		//body
	}
	else if(<boolExpr>)
	{
		//body
	}
	else
	{
		//body
	}
--------------------------------------------------------
In c/c++: Every Non-Zer number treated as TRUE and zero treated as FALSE
---------------

 int a = 10;
 
 if( a = 15){
	printf("Hi");
 }
 else{
   printf("Bye");
 }

Ouput: Hi
--------

In Java: 
--------

 int a = 10;
 
 if( a = 15)//Error
 {
	SOP("Hi");
 }
 else{
   SOP("Bye");
 }

Ouput: ERROR
-------------------------------------------------------------------------------------
Switch statements:
-----------------------
Till Java4 : char, byte, short, int
From Java5: enum, Wrapper classes
From Java7: String

Syntax:
-----------

	switch(<var>)
	{
	
		case <label-1> :
					------
					------
	    case <label-2> :
					------
					------
		case <label-n> :
					------
					------
		default: 
					------
					------
	}

Example:
-----------

		int day = 4; // user input;

		switch (day) {
		case 1: {
			System.out.println("Monday");
			break;
		}
		case 2: {
			System.out.println("Tuesday");
			break;
		}
		case 3: {
			System.out.println("Wednesday");
			break;
		}
		case 4: {
			System.out.println("Thursday");
			break;
		}
		case 5: {
			System.out.println("Friday");
			break;
		}
		case 6: {
			System.out.println("Saturday");
			break;
		}
		case 7: {
			System.out.println("Sunday");
			break;
		}
		default:
			System.out.println("Are you CRAZY !!!");
		}

---------------------------------------------------------------
Loops?
