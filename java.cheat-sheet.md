
# Compilation 

	- Compile a class => javac -d <target dir> <java file>
	- Run a class file => in the target dir run: java pack1.pack2.packn.myclass 
	- Create a jar file => jar --create --verbose --file lib.jar com/mycompany/*.class
	  and same with options -c -v -f or with the tar style cvf
	-   

# Class Notes

	- you can't call inner class's B constructor from a non-static outer class 
	  static method as inner classes are tied to the class A instance => Fix: change B to static 
	  class
	
	## Constructors
		
	- call one constructor inside another constructor of this class with this 
	- values are initialized 
	- constructor can contain a initialization block { } 
	- a class gets an empty constructor if no constructor is defined
	- if class contains a non-empty constructor then empty constructor must be 
	  specified explicitly
	- class can contain a static block for initialization 

# Call by value 

	- a call void f(A a) { a = new A(); } does change parameter a
	- 

# Input Output

	- For io use Scanner or Console classes and System.in
