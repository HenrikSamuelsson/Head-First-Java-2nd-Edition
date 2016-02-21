# Head First Java
Notes and exercises related to the book Head First Java, 2nd Edition.

## Exercise Solutions
Discussions and links to code for various exercises from the book.  
### Chapter 1 - A Quick Dip
#### Page 9 - Writing a class with main  
Typing, compiling and running of a program called [MyFirstApp](/workspace/Ch01 My First App/src/MyFirstApp.java). The output of this program will be:  
```
I Rule!
The World!
```
#### Page 12 - Example of a while loop  
Typing, compiling and running of a program called [Loopy](/workspace/Ch01 Loopy/src/Loopy.java). The output of this program will be:  
```
Before the Loop
In the Loop
Value of x is 1
In the Loop
Value of x is 2
In the Loop
Value of x is 3
This is after the loop
```

### Chapter 2 - Classes and Objects  

#### Page 42 - Be the Compiler
The code about tape decks will not compile because an object, called t, is used without being created. A fixed version of the code can be found [here](/workspace/Ch02 Tape Deck/src/TapeDeckTestDrive.java). The output of this program will be:  
```
tape playing
tape recording
```

The code about DVD players will not compile because an method is called that isn't defined in the class DVDPlayer. A fixed version of the code can be found [here](/workspace/Ch02 DVD Player/src/DVDPlayerTestDrive.java). The output of this program will be:  
```
DVD playing
DVD recording
```

### Chapter 4 - Methods use Instance Variables

#### Page 87 - Sharpen your pencil  
Assume that the method given below.  
```
int calcArea(int height, int width) {
	return height * width;
}
```
Example of legal statements that use the method are then the following.  
```
int a = calcArea(7, 12);
```
```
short c = 7;
calcArea(c, 12);    // ok because a short will always fit in an int  
```
```
calcArea(2, 3);    // it is ok to not use the return value for anyhthing
```
Statements that would be illegal are for example the following.  
```
int d = calcArea(57);  // one of the arguments are missing 
```
```
long t = 42;
int a = calcArea(t, 12);  // must cast the long to an in since t can be to big to fit in the int
```
```
int g = calcArea();	 // both arguments are missing
```
```
calcArea();  // both argumentsa are missing
```
```
byte h = calcArea(4, 20);  // the result may not fit in an byte variable since it is of type int
```
```
int j = calcArea(2, 3, 5);
```
