using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Exam_Three
{
    class Program
    {
        static void Main(string[] args)
        {
            string season = Console.ReadLine().ToLower();
            string gender = Console.ReadLine().ToLower();
            int students = int.Parse(Console.ReadLine());
            int nights = int.Parse(Console.ReadLine());

            string sport = "";
            double nightPrice = 0;

            if (season == "summer")
            {
                if (gender == "boys")
                {
                    sport = "Football";
                    nightPrice = students * nights * 15;
                    if (students >= 50)
                    {
                        nightPrice = nightPrice * 0.5;
                    }
                    else if (students < 50 && students >= 20)
                    {
                        nightPrice = nightPrice * 0.85;
                    }
                    else if (students < 20 && students >= 10)
                    {
                        nightPrice = nightPrice * 0.95;
                    }
                }
                else if (gender == "girls")
                {
                    sport = "Volleyball";
                    nightPrice = students * nights * 15;
                    if (students >= 50)
                    {
                        nightPrice = nightPrice * 0.5;
                    }
                    else if (students < 50 && students >= 20)
                    {
                        nightPrice = nightPrice * 0.85;
                    }
                    else if (students < 20 && students >= 10)
                    {
                        nightPrice = nightPrice * 0.95;
                    }
                }
                else if (gender == "mixed")
                {
                    sport = "Swimming";
                    nightPrice = students * nights * 20;
                    if (students >= 50)
                    {
                        nightPrice = nightPrice * 0.5;
                    }
                    else if (students < 50 && students >= 20)
                    {
                        nightPrice = nightPrice * 0.85;
                    }
                    else if (students < 20 && students >= 10)
                    {
                        nightPrice = nightPrice * 0.95;
                    }
                }
            }
            else if (season == "winter")
            {
                if (gender == "boys")
                {
                    sport = "Judo";
                    nightPrice = students * nights * 9.60;
                    if (students >= 50)
                    {
                        nightPrice = nightPrice * 0.5;
                    }
                    else if (students < 50 && students >= 20)
                    {
                        nightPrice = nightPrice * 0.85;
                    }
                    else if (students < 20 && students >= 10)
                    {
                        nightPrice = nightPrice * 0.95;
                    }
                }
                else if (gender == "girls")
                {
                    sport = "Gymnastics";
                    nightPrice = students * nights * 9.60;
                    if (students >= 50)
                    {
                        nightPrice = nightPrice * 0.5;
                    }
                    else if (students < 50 && students >= 20)
                    {
                        nightPrice = nightPrice * 0.85;
                    }
                    else if (students < 20 && students >= 10)
                    {
                        nightPrice = nightPrice * 0.95;
                    }
                }
                else if (gender == "mixed")
                {
                    sport = "Ski";
                    nightPrice = students * nights * 10;
                    if (students >= 50)
                    {
                        nightPrice = nightPrice * 0.5;
                    }
                    else if (students < 50 && students >= 20)
                    {
                        nightPrice = nightPrice * 0.85;
                    }
                    else if (students < 20 && students >= 10)
                    {
                        nightPrice = nightPrice * 0.95;
                    }
                }
            }
            else if (season == "spring")
            {
                if (gender == "boys")
                {
                    sport = "Tennis";
                    nightPrice = students * nights * 7.20;
                    if (students >= 50)
                    {
                        nightPrice = nightPrice * 0.5;
                    }
                    else if (students < 50 && students >= 20)
                    {
                        nightPrice = nightPrice * 0.85;
                    }
                    else if (students < 20 && students >= 10)
                    {
                        nightPrice = nightPrice * 0.95;
                    }
                }
                else if (gender == "girls")
                {
                    sport = "Athletics";
                    nightPrice = students * nights * 7.20;
                    if (students >= 50)
                    {
                        nightPrice = nightPrice * 0.5;
                    }
                    else if (students < 50 && students >= 20)
                    {
                        nightPrice = nightPrice * 0.85;
                    }
                    else if (students < 20 && students >= 10)
                    {
                        nightPrice = nightPrice * 0.95;
                    }
                }
                else if (gender == "mixed")
                {
                    sport = "Cycling";
                    nightPrice = students * nights * 9.50;
                    if (students >= 50)
                    {
                        nightPrice = nightPrice * 0.5;
                    }
                    else if (students < 50 && students >= 20)
                    {
                        nightPrice = nightPrice * 0.85;
                    }
                    else if (students < 20 && students >= 10)
                    {
                        nightPrice = nightPrice * 0.95;
                    }
                }
            }

            Console.WriteLine("{0} {1:f2} lv.", sport, nightPrice);
        }
    }
}
