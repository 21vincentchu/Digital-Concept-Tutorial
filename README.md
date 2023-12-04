# How to create an object in C#, by Vincent Chu

Summary: In this tutorial, I will be going the process of making an object class. While the syntax will not be all the same, the 
         theory and context behind the coding will be the same throughout most object oriented programming

Target Audience: This is for beginning coders who have started out coding in C# or JAVA, who are just in the phase of learning coding. I hope
                 this code is useful for other upcoming students, who people in general who are beginning to code in C# or Java


### Step 1: 
We need to create a class called Person. The class will be a blueprint to creating our person object. 
                  
### Step 2: 
We need to declare fields. These are variables that are UNIQUE to the object and to the class. 
 
### Step 3:
after declaring feilds, we declare our constructor. This will BUILD the object for us with all the field a person should have. 

### Step 3A:
We name the constructor the same as our file name. so it will be public Person.

### Step 3B: 
We assign the argument variable names, to the field names we made. 

### Step 4:
We go back to our main, make variables for our person object

### Step 4A: 
We call the Person class to make the person object. We do this by using the keyword new.

### Step 5:
We have finished! You have learned how to create a simple person object in C#


```
//Step 1: Make a class called Person
public class Person
{
    //Step 2: We declare our fields, which are attributes / variables to the person and object. 
    string name;
    string height;
    string gender;


    //Step 3: We declare a constructor to take the variables, takes in arguments, and creates the person object 
    public Person(string Name, string Height, string gender) //Step 3A
    {
        //Step 3B
        name = Name;
        height = Height;
        gender = Gender;
    }
}
class Program
{
    static void Main(string[] args)
    {
        //Step 4
        //This is the main program where all programs start in C#.
        //Here we have collected information about myself.
        string name = "Vincent Chu";
        string height ="5'8";
        string gender = "male";

        //We create the object, by calling the person class, followed by variable name, the new keyword to create object. then we call constructor               person. In parenthesis, we have the arguments necessary for the constructor to make our person object.

        //Step 4A
        Person vincent = new Person(name, height, gender);
    }
}



```
