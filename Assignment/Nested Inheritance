An interface which is declared inside another interface or class is called nested interface. They are also known as inner interface. Since nested interface cannot be accessed directly, the main purpose of using them is to resolve the namespace by grouping related interfaces related interface and class) together. This way, we can only call the nested interface by using outer class or outer interface name followed by dot( . ), followed by the interface name

                      code
                      
  public class Demo1 {
  public static void main(String[] args){
  C ob = new C();
  ob.method();
}
}

  class A{

  protected interface B{
  void method();
}
}


 class C implements A.B{
 public void method() {
 System.out.println("Demo: interface nested inside a class");
}
}

  Output : Demo: interface nested inside a class
