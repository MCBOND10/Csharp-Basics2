## Csharp Basics Round 2: Document

~~~C#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.IO;

namespace Document
{
    class Document
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Document");
            Console.WriteLine("\n\n");

            string doc_name;
            Console.Write("Please input the name of the document below:\n");
            doc_name = Console.ReadLine();
            doc_name += ".txt";
            Console.WriteLine("\nThis will be the name of your document: '{0}'.", doc_name);

            string doc_content;
            Console.Write("\nPlease input the content of the document below:\n");
            doc_content = Console.ReadLine();
            Console.WriteLine("\nThsi will be the content displayed inside of your document:\n{0}", doc_content);

            //StreamWriter sw = new StreamWriter(@"C:\Users\MCB10\Desktop\School Work\IT2040\Projects\Mod4\{0}", doc_name);
            //I couldnt get this to work. The intent was for the user inputted document name to be added to the end such as 'blankdoc.txt'.

            StreamWriter sw = new StreamWriter(@"C:\Users\MCB10\Desktop\School Work\IT2040\Projects\Mod4\IT2600document.txt");
            sw.WriteLine("{0}", doc_content);
            sw.Close();

            //I also failed to implement error handling before the assignment was due

        }
    }
}

~~~
