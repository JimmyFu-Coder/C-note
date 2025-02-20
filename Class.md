![[download.svg]]
# Encapsulation

Encapsulation allows you to ==hide details==. The details can still be accessed when necessary, but by intelligently encapsulating the details, large programs are made easier to understand, data is protected from inadvertent modification




# Inheritance
Inheritance in object-oriented programming allows you to form “==is a kind of==” relationships between these similar but different items. You will have defined a class hierarchy, which is a series of “is a kind of” relationships. You can view the class hierarchy graphically using a Unified Modeling Language (UML)–like class diagram, as shown in Figure

![[Pasted image 20250219095254.png]]

The more specialized type is called the ==derived type or the subtype==. The more general type is called the ==base type or the super type==.Derived types allow you to organize your classes into a coherent hierarchy where the derived types have greater specificity than their base types.

# Polymorphism
In the context of objects, polymorphism means that a single method or type can have many forms of implementation.


#  Instantiating a Class

```C#
public class Program

2. {

3.     public static void Main()

4.     {

5.         Employee employee1 = new Employee();

6.         Employee employee2;

7.         employee2 = new();

8.         //  Guidelines

			AVOID target-typed new expressions when the data type of the constructor is not obvious.

			CONSIDER use target-typed new expressions when the data type of the constructor is obvious.

9.         IncreaseSalary(employee1);

10.         IncreaseSalary(employee2);

11.     }

12.     // ...

13. }
```

Instance Fields
Instance Methods
This
Access Modifiers
1. fields should not be declared as public.
2. DO use properties for simple access to simple data with simple computations.
3. AVOID throwing exceptions from property getters.
4. CONSIDER using the same casing on a property’s backing field as that used in the property, distinguishing the backing field with an ==“_” prefix==.
5. DO favor automatically implemented properties over using fully expanded ones if there is no additional implementation logic.

Read-Only and Write-Only Properties
