# 5-ejercicios
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace TareaViernes

{
    internal class Program
    {
        static void Main(string[] args)

        {

            float suma = 0;

            int[] numeros = new int[6];

            for (int i = 0; i < numeros.GetLength(0); i++)
            {
                Console.WriteLine("valor de vector  " + "0" + "," + i);


                numeros[i] = Convert.ToInt32(Console.ReadLine());
            }

            for (int i = 0; i < numeros.GetLength(0); i++)
            {
                Console.Write("[" + i + "]" + "=" + numeros[i] + "  ");
            }
            Console.WriteLine();


            for (int i = 0; i < numeros.Length; i++)
            {
                suma += numeros[i];
            }

            Console.WriteLine();
            Console.WriteLine("El promedio es " + suma / numeros.Length);
            // intercambio de variables
            {
                int uff = 25;
                int off = 50;

                uff = uff + off;
                off = uff - off;
                uff = uff - off;
                Console.WriteLine("El nuevo valor de la variable 1 es" + "  " + uff);
                Console.WriteLine("El nuevo valor de la variable 2 es:" + "  " + off);
                Console.ReadLine();
                {

                    // numeros repetidos 
                    {
                        int[] lista = { 1, 3, 9, 4, 9, 16, 16, 8, 1, 4, 8, 8, 1, 5, 78, 56, 86, 78 };
                        bool repetidos = false;
                        for (var x = 0; x < lista.Length; x++)
                        {
                            int a = lista[x];
                            int c = x + 1;
                            for (int y = c; y < lista.Length; y++)
                            {
                                int b = lista[y];
                                if (a == b)
                                {
                                    repetidos = true;
                                    System.Console.WriteLine("El numero " + a + " esta repetido en la lista.");
                                }
                            }
                        }
                        if (repetidos == false)
                        {
                            System.Console.WriteLine("No hay ningun numero repetido.");
                        }
                        {

                            {
                                if (numeros[0] < numeros[1] & numeros[1] < numeros[2] & numeros[2] < numeros[3] & numeros[3] < numeros[4] & numeros[4] < numeros[5] & numeros[6] < numeros[7] & numeros[7] < numeros[8] & numeros[8] < numeros[9])
                                {
                                    Console.WriteLine("Los numeros están ordenados de menor a mayor");

                                }
                            }


                        }
                    }
                }
            }







        }
    }
}
