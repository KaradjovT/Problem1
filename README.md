using System;

class Program
{
    static void Main()
    {
        int s = int.Parse(Console.ReadLine());
        int d = int.Parse(Console.ReadLine());
        int Melons = 0;
        int Watermelon = 0;
        int Rezult = 0;
        for (int i = d; i > 0; i--)
        {
            if (s == 1)
            {
                Watermelon += 1;
            }
            if (s == 2)
            {
                Melons += 2;
            }
            if (s == 3)
            {
                Watermelon += 1;
                Melons += 1;
            }
            if (s == 4) 
            {
                Watermelon += 2;
            }
            if (s == 5)
            {
                Watermelon += 2;
                Melons += 2;
            }
            if (s == 6) 
            {
                Watermelon += 1;
                Melons += 2;
            }
            if (s == 7)
            {
                s = 0;
            }
            s++;
        }
        if (Watermelon> Melons)
        {
            Rezult = Watermelon - Melons;
            Console.WriteLine("{0} more watermelons",Rezult);
        }
        if(Melons>Watermelon)
	    {
            Rezult = Melons - Watermelon;
            Console.WriteLine("{0} more melons",Rezult);
	    }
        if (Watermelon == Melons)
        {
            Console.WriteLine("Equal amount: {0}",Melons);
        }
    }
}

