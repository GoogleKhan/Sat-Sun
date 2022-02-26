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














		
		
		
		
		
		