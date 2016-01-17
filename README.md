# cakes
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace CakeTycoonProblem
{
    class CakeTycoon
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
                int truffelCost = t * p;
                Console.WriteLine("truffelCost");
            }
            else if (numberCakesCan < n)
            {

            }


        }
    }
}
