# CSharp-Polymorphism

1) Polymorphism means "many forms" ,and it occurs when we have many class that are related to each other by inheritence
2) Inheritance lets us inherit fields and methods
3) Polymorphism use those methods to perform different tasks
4) This allows us to perform a single action in different ways.

=================================

# Method Overloading:
i)In this case we define multiple methods with the same name by changing their parameters
ii) This can be performed either within a class as well as between parent and child classes
iii) We can call the appropriate method at appropriate place.
iv) Return types are not considered
                   public string Test()             //invalid
                   
                   
=================================
Let us consider 5 methods

   public void Test()
   public void Test(int i)
   public void Test(string s)
   public void Test(int i,string s)
   public void Test(string s,int i)
   
   static void Main(string[]args)
   {
   Program p= new Program;
   p.Test();
   p.Test(123);
   p.Test("Sajeev");
   p.Test(123,"Sajeev");
   p.Test("Sajeev",123);
   
   ====================================================
   
   using System;

class load
{
    public int Add(int a,int b)
    {
        int sum=a+b;
        return sum;
    }
    public int Add(int a,int b,int c)
    {
        int sum=a+b+c;
        return sum;
    }
    public static void Main(string[]args)
    {
        load Obj = new load();
        int sum1 = Obj.Add(1, 2);
        Console.WriteLine("sum of two is:" +sum1);                //sum of two is:3
        int sum2= Obj.Add(4,5,6);
        Console.WriteLine("Sum of three is : " +sum2);            //Sum of three is : 
    }
 }
 
 =========================================================
 
 # Method Overriding
 
 i)In this case we define multiple methods with the same name and same parameters
ii) This can be performed only between parent and child classes and never be performed in the same class


------------------------

class1
public virtual void Test()      //overriadable
class2:class1
public override void Test()     //overriding

------------------------
class base_class
{
    public void gfg();
}

class derived_class : base_class
{
    public void gfg();
}

class Main_Method
{
 static void Main()
 {
    derived_class d = new derived_class();
    d.gfg();
 }
}

----------------------------

using System;

class base_class
{
    public  virtual void show()
    {
        Console.WriteLine("Hey Honey :* ");
    }
}

class derived_class : base_class
{
    public override void show()
    {
        Console.WriteLine("I'm Home !");
    }
}

class Main_Method
{
  public static void Main()
 {
    base_class Obj = new base_class();
    Obj.show();
    Obj = new derived_class();                                     //Hey Honey :*
    Obj.show();                                                   //I'm Home !
 }
   
   
   
   
   
   
   
   
