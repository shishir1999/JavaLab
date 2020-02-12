Default methods can be provided to an interface without affecting implementing classes as it includes an implementation. If each added method in an interface is defined with implementation, then no implementing class is affected. An implementing class can override the default implementation provided by the interface.

   CODE|:    
  
      interface Test
     { 
 
      public void square(int a); 

     default void show() 
    { 
     System.out.println("Default Method Executed"); 
    } 
    } 

     class TestClass implements Test
    { 
 
     public void square(int a) 
    { 
     System.out.println(a*a); 
    } 

     public static void main(String args[]) 
    { 
     TestClass d = new TestClass(); 
     d.square(4); 
     d.show(); 
     } 
     } 
