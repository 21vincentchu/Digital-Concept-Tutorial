# How to create an object in C#, by Vincent Chu

Summary: In this tutorial, I will be going the process of making an object class. While the syntax will not be all the same, the 
         theory and context behind the coding will be the same throughout most object oriented programming

Target Audience: This is for beginning coders who have started out coding in C# or JAVA, who are just in the phase of learning coding. I hope
                 this code is useful for other upcoming students, who people in general who are beginning to code in C# or Java


### Step 1: 
         We need to create a class called Person.The class will be a blueprint to creating our person object. 
                  
### Step 2: 
         We need to declare fields. These are variables that are UNIQUE to the object and to the class. This will include name, height, and                         gender. All being of type string
### Step 3:
         after declaring feilds, we declare our constructor. This will BUILD the object for us with all the field a person should have. 
### Step 3A:
         We name the constructor the same as our file name. so it will be public Person. After we have arguments. It will take in three. Name, height,              gender. All of type String
### Step 3B: 
         We assign the argument variable names, to the field names we made. 
### Step 4: 
         We go back to our main, we call the Person class to make the person object. We do this by using the keyword new. we also send in argument to             create the object
### Step 5:
         We have finished! You have learned how to create a simple person object in C#


```
class Program
{
    static void Main(string[] args)
    {
        //This is the main program where all programs start in C#.
        //Here we have collected information about myself.
        string name = "Vincent Chu";
        string height ="5'8";
        string gender = "male";

        //We create the object, by calling the person class, followed by variable name, the new keyword to create object. then we call constructor               person. In parenthesis, we have the arguments necessary for the constructor to make our person object.

        Person vincent = new Person(name, height, gender);
    }
}

//A different class that is specific to making the person object. 

public class Person
{
    //We declare our fields, which are attributes / variables to the person and object. 
    string name;
    string height;
    string gender;

    //We declare a constructor to take the variables, takes in arguments, and creates the person object 
    public Person(string Name, string Height, string gender)
    {
        name = Name;
        height = Height;
        gender = Gender;
    }

```
