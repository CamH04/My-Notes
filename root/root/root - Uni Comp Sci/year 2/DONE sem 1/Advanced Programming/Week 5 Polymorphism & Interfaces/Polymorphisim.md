# Polymorphisim
Overriding a method within a class

*   Polymorphism refers to the ability to have a method inherited by parent classes but  
    having it do different things – one method, many uses

Virtual , Abstract 

*   The override modifier is required to extend or modify an inherited abstract or virtual  
    method or property.  
     - Abstract methods do not have an implementation, forcing the derived classes to override  
    them.  
    \- Virtual methods have an implementation, giving derived classes the option of overriding  
    them.

Method redefinition occurs when an inherited method in a derived class intends to hide  
rather than extend the base class method of the same name.  
Where the override modifier extends the base class method, the new modifier hides it.