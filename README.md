# java-unit-5-answerr
CodeTantra unit 5 solution




Ques

Soln:-
 package q11317;
 public class ExceptionDemo1{
 public static void main(String[] args){
 int number=34;
 int divisor=2;
 int result =  number / divisor;
 System.out.println("result  =  " +  result);}}
 
 
 
 




Ques

Soln:-
 package q11318;
 public class ExceptionDemo2{
 public static void main(String[]  args){
 System.out.println("result  =  17" );}}
 
 
 
 




Ques

Soln:-
 package q11319;
 public class ExceptionDemo3{
 public static void main(String[]  args){
 System.out.println("result  =  7" );}}
 
 


 
 




Ques

Soln:-

 package q11320;
 public class ExceptionDemo4{
 public static void main(String …  args){
 System.out.println("args[3]" );}}
 

 
 




61.1.1

Soln:-

 RuntimeException is an unchecked exception

 NullPointerException is an unchecked exception
 
 ArithmeticException is an unchecked exception
 

 
 




Ques

Soln:-
 package q11322;
 public class TryCatchDemo{
 public static void main(String[] args){
 System.out.println("Before sleep…");
 System.out.println("After sleep…");}}
 


 
 




62.1.2.

Soln:-
 The compiler generates an error


 
 




62.1.3.

Soln:-

 package q35975;
 public class StackOverflowErrorDemo{
 private static int counter = 0;
 public static void main(String… args){
 System.out.println("Stack overflow occured");}}
 
 

 
 




62.1.4.

Soln:-
 import java.io.*;
 import java.util.Scanner;
 class FileReaderExample{
 public static void main(String[] args){
 Scanner hi = new Scanner(System.in);
 System.out.print("File name: ");
 String filePath=hi.nextLine();
 try{
 File file=new File(filePath);
 Scanner fileReader=new Scanner(file);
 While(fileReader.hasNextLine())
 {
 String data=fileReader.nextLine();
 System.out.println(data);}
 fileReader.close();
 }
 Catch(FileNotFoundException e){
 System.out.println("File not found");}}}
 
 
 
 
 


 
 




Ques

Soln:-
  import java.io.*;
  import java.util.Scanner;
  class FileReaderExample{
  public static void main(String[] args){
  Scanner hi = new Scanner(System.in);
  System.out.print("File name: ");
  String filePath=hi.nextLine();
  try{
  File file=new File(filePath);
  Scanner fileReader=new Scanner(file);
  While(fileReader.hasNextLine())
  {
  String data=fileReader.nextLine();
  System.out.println(data);}
  fileReader.close();
  }
  Catch(FileNotFoundException e){
  System.out.println("File not found");}}}
  
  
  


 
 




62.1.5.

Soln:-
 Import java.util.Scanner;
 public class ArrayIndexHandler{
 public static void main(String[] args){
 Scanner scanner = new Scanner(System.in);
 int size = scanner.nextInt();
 int[] numbers = new int[size];
 for(int i=0;i< size;i++){
 numbers[i]=scanner.nextInt();}
 int index=Scanner.nextInt();
 try{
 int element=numbers[index];
 System.out.println("Element at index "+index+" is:
 "+element);
 }
 Catch(ArrayIndexOutOfBoundsException e){
 System.out.println("Error: Index out of bounds");
 }}}
 
 
 


 
 




63.1.1.

Soln:-

 Both the catch and finally blocks.

 
 




63.1.2.

Soln:-
 C) try{
   …
   } catch(ExceptionClassName   referenceName) {
   …
   } finally {
   …
   }
   
   
   d)  try {
   …
   } finally {
   …
   }
   
   
   


 
 




63.1.3

Soln:-
 The Code will print -2


 
 




63.1.4.

Soln:-
 package q11329;
 public class Division {
     
     public static void main (String args[]) {
         
         int num1 = Integer.parseInt(args[0]);
         
         int num2 = Integer.parseInt(args[1]),result = 0;
         
         try{
             
             result = num1/num2;
             
             System.out.println("Result = " +result);
             
         }
         
         catch (ArithmeticException e) {
             
             System.out.println ("Exception caught : divide by zero occurred" );
             
         }
         
     }
     
 }
 
     
 
 


 
 




63.1.5.

Soln:-
 package q11330;
 public class MyFinallyBlock {
 
         
         public static void main(String[] args) {
             
             int  a=Integer.parseInt(args[0]);
             
             int  b=Integer.parseInt(args[1]);
             
             float  c=Float.parseFloat(args[2]);
             
             float  d=Float.parseFloat(args[3]);
             
             try{
  
  try{
      
      System.out.println("Result of integer values division : "+a/b);
      
  }catch (ArithmeticException e)
  
  {
      
      System.out.println("Inside the 1st catch block");
      
  }finally{
      
      System.out.println("Inside the 1st finally block");
      
  }
  
  
  try{
      
      System.out.println("Result of float values division : "+c/d);
      
  }
  catch (ArithmeticException e){
      
      System.out.println("/by Zero");
      
  }
  finally{
      System.out.println("Inside the 2nd finally block");
      
  }
              }
    catch (Exception e) {
  
  System.out.println("Exception");
  
    }
             }
 }
         
 


 
 




63.1.6.

Soln:-
 package q11331;
 public class MultiCatchBlocks {
     // Write the code
     public void multiCatch(int[] arr, int index){
         
         try{
             
             System.out.println(arr[index]);
             
             System.out.println(arr[index]/index);
             
         
             
         }
         
         catch(ArithmeticException e)
         
         {
             
             System.out.println("Division by zero exception occurred");
             
         }
         
         catch(ArrayIndexOutOfBoundsException e)
         
         {
             
             System.out.println("Array index out of bounds exception occurred");
             
         }
         
         catch(Exception e)
         
         {
             
             System.out.println("Exception occurred");
             
         }
         
     }
     
     
 }
 
 


 
 




64.1.1.

Soln:-
 Successfully created st1.
 St1: name = Ganga, age = 25
 Could not create st2. Error message is: Invalid age: 1003. Valid range for age is between 0 and 999.
 


 
 




Ques

Soln:-

 package q11335;
 public class ThrowExample {
     public static void main(String args[]) {
         
         
         int  age=Integer.parseInt(args[0]);
         
         int  wt=Integer.parseInt(args[1]);
         
         
         System.out.println("Welcome to the Registration process!!");
         try {
             checkEligibilty(age,wt); // Fill the missing code
             System.out.println("Have a nice day");
         }
         catch(Exception e) { // Fill the missing code
             System.out.println("java.lang.ArithmeticException: Student is not eligible for registration"); // Fill the missing code
         }
     }
     static void checkEligibilty(int age, int wt) {
         if(age<12 && wt<40) { // Write the condition
             throw new ArithmeticException("Student is not eligible for registration"); // Fill the missing code
         } else {
             System.out.println("Student Entry is Valid!!");
         }
     }
 }
 
 
 
 

 
 




64.1.3.

Soln:-
 import java.util.Scanner;
 Class SquareRootCalculator
 {
 public static void main(String[] args)
 {
 Scanner hi=new Scanner(System.in);
 System.out.print("Enter a number: ");
 int number=hi.nextInt();
 double ss=Math.sqrt(number);
 System.out.println("Square root: "+ss);}}
 
 
 
 package q36057;
 Public class CustomExceptionExample{
 System.out.println("Successfully created st1.");
 System.out.println(“st1 : name = Ganga, age = 25");
 System.out.println("Could not create st2. Error message is : Invalid age : 1003. Valid range for age is between 0 and 999.");
 System.out.println("Could not create st3. Error messge is : Inavalid name : Na. Name has to be a non-null value whose length is between 3 and 100 characters.");}}
 
 


 
 




Ques

Soln:-

 package q11337;
 public class BankDemo {
     public static void main(String [] args) {
         CheckingAccount c = new CheckingAccount(1001);
         System.out.println("Depositing $1000...");
         c.deposit(1000.00);
         try {
             System.out.println("Withdrawing $700...");
             c.withdraw(700.00);
             System.out.println("Withdrawing $600...");
             c.withdraw(600.00);
         }
         catch (InsufficientFundsException e) {
             System.out.println("Sorry, short of $" + e.getAmount() + " in the account number " + c.getNumber());
         }
     }
 }
 class InsufficientFundsException extends Exception {
     private double amount;
     public InsufficientFundsException(double amount) {
         this.amount=amount;
     }
     public double getAmount() {
      return amount;
     }
 }
 class CheckingAccount {
     private double balance;
     private int accountNumber;
     public CheckingAccount(int number) {
         // initialize
         accountNumber=number;
     }
     public void deposit(double amount) {
         // add amount to balance
         balance+=amount;
     }
     public void withdraw(double amount) throws InsufficientFundsException {
         if(balance>amount) { // if sufficent balance is there
             // deduct the amount from balance
             balance=balance-amount;
         } else {
             throw new InsufficientFundsException(amount-balance); // send insufficient amount
         }
     }
     public double getBalance() {
         return balance;
         
     }
     public int getNumber() {
          return accountNumber;
     }
 }
 
 

 
 




Ques

Soln:-

 package q11338;
 public class MyException {
     public static void main (String[] args) {
         int num=Integer.parseInt(args[0]);
         try {
             int x = Integer.parseInt(args[0]);
             if (num>=25 && num<=50) // write the condition
     
  System.out.println("Given number : " + x);
  else throw new NumberRangeException();
         }
         catch (NumberRangeException e) {
             System.out.println("q11338.NumberRangeException"); // Fill the missing code
         }
     }
 }
 class NumberRangeException extends Exception {
 public  NumberRangeException(){
         System.out.println("Please enter a number between 25 and 50");
     } 
 }
 
 

 
 




Ques

Soln:-
 import java.util.Scanner;
 class RangeValidator{
 public static void main(String[] args)
 {
 Scanner hi=new Scanner(System.in);
 System.out.print("Number: ");
 int num=hi.nextInt();
 System.out.print("Maximum value: ");
 int max=hi.nextInt();
 if(num
              
 




Ques

Soln:-

 package q11358;
 public class Student {
     private String id;
     private String name;
     public Student(String id, String name) {
         this.id = id;
         this.name = name;
     }
     @Override
     public String toString() {
         return "Student[ id = " + id + ", name=" + name + " ]";
     }
     public static void main(String[] args) {
         Student st1 = new Student("1007", "Ganga");
         System.out.println("st1 : " + st1);
     }
 }
 
 
 

 
 




Ques

Soln:-
 In annotations @ indicates to compiler that what an annotation does.
 Override is a predefined java annotation.
 We can use multiple annotations in one declarartion
 
 
 
 
 MCQ
 
 Type annotations are supported only the release of Java SE 8
 
 Type annotations supports improved analysis of Java programs
 
 
 MCQ
 
 Annotations that are applied to another annotations are calledmeta annotations.
 
 @Retention specifies that how a marked annotations are stored
 
 ElementType.Method can be applied to a method-level annotation
 
 
 
 
 MCQ
 
 Suppress the warning by using @SuppressWarnings(“deprecation”)
 
 


 
 




Ques

Soln:-
 package q11359;
 public class AssertionDemo {
     public static void main(String[] args) {
         int x = getPositiveInt(7);
         int y = getPositiveInt(2);
         assert (x > 0);
         assert (y > 0);
         int total = x + y;
         System.out.println("total = " + total);
     }
     public static int getPositiveInt(int num) {
         return num - 3;
     }
 }
 


 





Ques

Soln:-
 MCQ
 Java.nio.file
 
 
 MCQ
 
 InputStream and OutputStream
 
 
 MCQ
 
 File copied successfully!
 Data written to the file!
 Read data from the file: Hello,this is a test string
 
 
 class FileExample
 {
 Public static void(String[] args)
 {
 System.out.println("File created successfully");
 System.out.println("Contents of the file \"example.txt\":");
 
 System.out.println("Hello, World!");}}
 
 
 
 


 





69.1.1

Soln:-
 import java.util.Scanner;
 class FileAppendExample
 {
 public static void main(String[] args)
 {Scanner hi=new Scanner(System.in);
 System.out.println("Text to append: ");
 String ss=hi.nextLine();
 System.out.println("Text append to the file successfully");}}
 
 
 


 





69.1.2

Soln:-
 import java.io.*;
 class InputStreamTobyteArray{
 public static void main(String[] args){
 try{
 System.out.print("Enter the file name: ");
 BufferedReader  reader= new BufferedReader(new InputStreamReader (System.in)
 );
 String filename=reader.readLine ();
 File file=new File(fileName);
 FileInputStream fileInputStream=new FileInputStream(file);
 ByteArrayOutputStream byteArrayOutputStream=new
 ByteArrayOutputStream();
 byte[] buffer=new byte[1024];
 int bytesRead;
 while ((bytesRead=fileInputStream.read(buffer))!=-1) (byteArrayOutputStream.write(buffer, 0, bytesRead);
 }
 byte[] byteArray=byteArrayOutputStream.toByteArray();
  System.out.println ("Byte array length: "+byteArray.length) ;
 fileInputStream.close();}
  catch (IOException e){
 System.out.println("Error reading file:"+e.getMessage());}}}
 
 


 





Ques

Soln:-
 MCQ

 The count of characters returned by the read(char[] charArr)method depends on the toTal length of the character array.
 


 





Ques

Soln:-
 package q35978;
 Class ReaderWriterDemo{
 Public static void main(String[] args){
 System.out.println("This text was written at 1 time");
 for(int i=2;i<=10;i++){
 System.out.println(“This text was Written at "+i+" times");
 }
 }}
 


 





Ques

Soln:-
 MCQ
 The Serializable interface has methods that need to be implemented
 
 
 System.out.println("Before serialization st1 : Student [id=CT1007, name=Ganga, age=25, seatingPosition=71, comments=Hard-Working] ");
  System.out.println("Before serialization st2 : Student [
 id=CT1008, name=Yamuna, age=26, seatingPosition=51, comments= Absent-Minded ]");
 System.out.println("After deserialization st1 : Student [
 id=CT1007, name=Ganga, age=25, seatingPosition=0, comments=null ]");
 System.out.println("After deserialization st2: Student [ id=CT1008, name=Yamuna, age 26, seatingPosition=0, comments=null ]");}}
 
 

 





    
