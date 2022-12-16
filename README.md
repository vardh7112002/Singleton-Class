                                                                                     -Singleton Class


 class A {
    private static A obj = new A(); 
    private A()
    {
        
    }
    static A getObject(){
        return obj;
    }
};
 public class B {
     public static void main(String[] args) {
    //  A a1= new A();
        A a1= A.getObject();
        A a2=A.getObject();
        System.out.println(a1==a2);
     }
};
