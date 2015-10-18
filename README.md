# Learning-Java
......................
	Encapsulation:
Example---
public class selfTry{
private String name;
private int age;
private float salary;
public String getname()
{
    return name;
}
public int getage()
{
    return age;
}
public float getsalary()
{
    return salary;
}
public void setname(String newname)
{
    name=newname;
}
public void setage(int newage)
{
    age=newage;
    
}
public void setsalary(float newsalary)
{
    salary=newsalary;
}
}
public class Record {
    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        selfTry e1=new selfTry();
   e1.setname("ali");
   e1.setage(22);
   e1.setsalary(10000);
   System.out.println("name is="+e1.getname());
   System.out.println("age is="+e1.getage());
   System.out.println("salary is="+e1.getsalary());
       
    }
}   
	Inheritance
Example---
  public class calculation{
            int z;
            public void addition(int x, int y){
                z=x+y;
                System.out.println("sum of two values="+z);
            }
            public void substraction(int x, int y){
                z=x-y;
                System.out.println("substraction of two values is="+z);
            }
    }
    public class mycalculation extends calculation{
        public void multiplication(int x, int y)
        {
            z=x*y;
            System.out.println("multiplication of two values="+z);
        }
    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
    mycalculation cal=new mycalculation();    
    int a=20;
    int b=10;
    cal.addition(a,b);
    cal.substraction(a,b);
    cal.multiplication(a,b)    
    }    
}
<><><><><><><><>---------------------<><><><><><><><>
	Abstract
abstract class A {
     void callme()
    void calltome()
    {	
        
    }
}
class B extends A {
    void callme()
    {
        System.out.println("B implement to callme");
    }
}
 class abstractDispaly{         
    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        
       B b=new B ();
       b.callme();
       b.calltome()
  }
    }
<><><><><><><><>……………………<><><><><><><><><>

	Polymorphism

	Example
class Animal{
    public Animal(){
        System.out.println("a animal can created=");
    }
public void sleep(){
    System.out.println("a animal sleep=");
}
public void eat(){
    System.out.println("a animal eat something=");
}
}
class Cat extends Animal{
    public Cat()
    {
       super();
       System.out.println("a new animal cat created=");
    }
    public void sleep()
    {
        System.out.println("a cat can sleep=");
    }
    public void eat()
    {
        System.out.println("a cat can eat someting=");
    }
}
public Horse extends Animal{
public Horse(){
super();
System.out.println("a new animal horse creaed=");
}
public void sleep()
{
System.out.println("a horse can sleep=");
}
public void eat()
{
System.out.println("a horse eat something=");
}
}
public class DisPolymorphism {
    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
    Animal animal = new Animal();
    Cat cat = new Cat();
    Horse horse = new Horse();
    Animal cat1 = new Animal();
    Animal horse1 = new Animal();
  System.out.println("finally dispaly classes=");
  animal.sleep();
  animal.eat();
  cat.sleep();
  cat.eat();
  horse.sleep();
  horse.eat();
  cat1.sleep();
  cat1.eat();
  horse1.sleep();
  horse1.eat();
    }  
}







      <><><><><><><><>-------------------<><><><><><><><><>

