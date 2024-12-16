# 16
using System;
using System.Collections;

class Program
{
    static void Main()
    {
        ArrayList collection = new ArrayList();
        collection.Add(10);
        collection.Add("Hello");
        collection.Add(true);
        collection.Add(3.14);
        collection.Add(-5);
        collection.Add(-2.71);

        foreach (var item in collection)
        {
            Console.WriteLine(item);
        }

        Console.WriteLine($"\nКоличество элементов в коллекции: {collection.Count}");

        collection.Insert(1, "Inserted String");

        foreach (var item in collection)
        {
            Console.WriteLine(item);
        }

        collection.Remove(10);

        foreach (var item in collection)
        {
            Console.WriteLine(item);
        }

        collection.Reverse();

        foreach (var item in collection)
        {
            Console.WriteLine(item);
        }

        string[] stringArray = new string[] { "One", "Two", "Three" };
        collection.AddRange(stringArray);

        foreach (var item in collection)
        {
            Console.WriteLine(item);
        }
    }
}
