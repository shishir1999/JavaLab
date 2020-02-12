An exception (or exceptional event) is a problem that arises during the execution of a program. When an Exception occurs the normal flow of the program is disrupted and the program/Application terminates abnormally, which is not recommended, therefore, these exceptions are to be handled.

An exception can occur for many different reasons. Following are some scenarios where an exception occurs.

A user has entered an invalid data.

A file that needs to be opened cannot be found.

A network connection has been lost in the middle of communications or the JVM has run out of memory.

CODE||:

      class InvalidAgeException extends Exception{  
      InvalidAgeException(String s){  
      super(s);  
    }  
    }  
     class TestCustomException1{  

     static void validate(int age)throws InvalidAgeException{  
     if(age<18)  
     throw new InvalidAgeException("not valid");  
     else  
     System.out.println("welcome to vote");  
 }  
 
    public static void main(String args[]){  
    try{  
    validate(13);  
   } catch(Exception m){System.out.println("Exception occured: "+m);}  

     System.out.println("rest of the code...");  
}  
}
    Output:Exception occured: InvalidAgeException:not valid
           rest of the code...
