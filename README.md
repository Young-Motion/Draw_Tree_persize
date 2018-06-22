    using System;
    using System.Collections.Generic;
    using System.Linq;
    using System.Text;
    using System.Threading.Tasks;

    namespace ConsoleApp2
    {
        class Program
        {
            static void Main(string[] args)
            {//=========================================================
                    int width = 0;
                    double rowcount = 1;
                    int starcount = 0;
                    double spacecount = 0;
                    Console.WriteLine("please enter width of tree");
                    width = Convert.ToInt16(Console.ReadLine());
                    spacecount = (width / 2);
                    //tree builder
                    while (rowcount < width)
                    {
                        while (spacecount < width)
                        {
                            Console.Write(" ");
                            spacecount = spacecount + 1;
                        }

                        while (starcount < rowcount)
                        {
                            Console.Write("*");
                            starcount++;
                        }

                        rowcount++;
                        Console.WriteLine("");
                        starcount = 0;
                        spacecount = width / 2 + (Math.Round(rowcount / 2, 1));
                    }

                    //trunk builder
                    for (int b = 1; b < (width / 5); b++)
                    {
                        spacecount = width / 2 + width / 16;
                        while (spacecount < width)
                        {
                            Console.Write(" ");
                            spacecount = spacecount + 1;
                        }

                        Console.Write("|");
                        spacecount = width - width / 16;
                        while (spacecount < width)
                        {
                            Console.Write(" ");
                            spacecount = spacecount + 1;
                        }

                        Console.WriteLine("|");
                    }
                Console.ReadLine();















                //==============================================================
        }
        }
    }
