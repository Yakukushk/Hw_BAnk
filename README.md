#Hw
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp2
{
    public class Student
    {
        string name;
        int age;
        public Student(string name)
        {
            this.name = name;
            Console.WriteLine("");
        }
        public Student(string name, int age) : this(name)
        {
            this.age = age;
            Console.WriteLine("");
        }

        void Study() { }
        void Read() { }
        void Write() { }
        void Relax() { }
        

    }
    public class GoodStudent : Student {

        public GoodStudent(string name, int age, string status) : base(name, age) {
            
            Console.WriteLine("Dima");
            Console.Write(age);
            Console.WriteLine(status);
        }

    }
    public class BadStudent : Student{
        public BadStudent(string name, int age, string status) : base(name, age)
        {
            Console.WriteLine("Baklan");
            Console.Write(age);
            Console.WriteLine(status);
        }
        
    }
    public class Debug  {
        static void Main(string[] args)
        {
            GoodStudent student = new GoodStudent("Dima", 13, " Exellent Student");
            BadStudent student1 = new BadStudent("Baklan", 13, " Worse Student");

           


        }

    }
    
}
