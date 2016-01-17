# cakes
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication1
{
    class Program
    {
        static void Main(string[] args)
        {
            int n = int.Parse(Console.ReadLine());    //amount of cakes Ivancho wants
            float c = float.Parse(Console.ReadLine());    //kilograms of flour needed to make one cake
            int f = int.Parse(Console.ReadLine());         //kilograms of flour available
            int t = int.Parse(Console.ReadLine());          //amount of truffles available
            int p = int.Parse(Console.ReadLine());          //price of one truffle

            float numberCakesCan = int.Parse(Console.ReadLine()); //Amount of cakes we have enough flour for 
            numberCakesCan = f / c;

            if (numberCakesCan > n)
            {
                Console.WriteLine("n");
                float truffelCost = int.Parse(Console.ReadLine());
                truffelCost = t * p;
                Console.WriteLine("{0}", truffelCost);

                //Console.WriteLine(" truffelCost"); // maybe?
                double cakePrice = float.Parse(Console.ReadLine());
                cakePrice = (truffelCost) / n * 1.25;
                Console.WriteLine("All products available, price of cake: {0}", cakePrice);


            }
            else if (numberCakesCan < n)
            {

            }
        }
    }
}
