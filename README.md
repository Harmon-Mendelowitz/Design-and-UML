# Java 3: Design and UML

#### Ex 3.1

![Q1](Java3Q1.png)

#### Ex 3.2

![Q2](Java3Q2.png)

#### Ex 3.2

![Q3](Java3Q3.pdf)

#### Ex 3.4

Employee e0 = new Employee ("Gullible Gus", "555-55-5678", 50000);  
  This works since e0 is a declared and instantiated as an Employee  
Employee e1 = new Customer ("Gullible Gus", "555-55-5678", 5);  
  This does not work since both employee and suctomer extend person but don't relate to each other  
Employee e2 = new Person("Zany Zoe", "112-12-1212");  
  This works since employee extends person  
Person p1 = new Customer ("Gullible Gus", "555-55-5678", 5);  
  Person variables can hold subclass instances  
Person p2 = (Person) e0;  
  Casting to a person will work  
Customer c1 = (Person) p1;  
  Casting to a person will work  
Customer c2 = p1;  
  Will also work since p1 without the casting is a 'new Customer'  
Person p3 = (Employee) e0;  
  Person variables can hold subclass instances  
Person p4 = e0;  
  Same as above  
