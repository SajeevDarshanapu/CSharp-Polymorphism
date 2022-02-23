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
