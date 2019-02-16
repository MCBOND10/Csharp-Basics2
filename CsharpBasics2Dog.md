## Csharp Basics Round 2: Dog

~~~C#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Dog
{
    class Dog
    {
        static void Main(string[] args)
        {
            string dog_name;
            string owner;
            string age1;
            int age;
            string gender;

            Console.WriteLine("What is the dog's name?");
            dog_name = Console.ReadLine();

            Console.WriteLine("You are the owner. What is your name?");
            owner = Console.ReadLine();

            Console.WriteLine("What is the gender of your dog?");
            gender = Console.ReadLine();

            Console.WriteLine("How old is your dog?");
            age1 = Console.ReadLine();
            age = Convert.ToInt32(age1);

            Console.WriteLine("If lost, call {0}. My name is {1}. I am a {2} and I am {3} year(s) old.", owner, dog_name, gender, age);
        }
    }
}

~~~

This is as far as I got on this assingment. I know that gender is supposed to be an enum. I know that each field is supposed to be within a constructor. I procrastinated and waited too long to work on the project. Then, when I started doing the project, internet went out so I couldnt proceed any further. I gave it my best shot with the time I had.
