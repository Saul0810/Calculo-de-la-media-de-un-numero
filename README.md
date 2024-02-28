# Calculo-de-la-media-de-un-numero
Un programa que pida al usuario 10 números reales de doble precisión, calcule su media y luego muestre los que están por encima de la media.

int cantidad = 10;
double[] numeros = new double[cantidad];
double suma = 0;
double media;


for (int i = 0; i < cantidad; i++)
{
    Console.WriteLine("Ingrese el numero: {0}", i + 1);
    numeros[i] = double.Parse(Console.ReadLine());
    suma = numeros[i];

}
media = suma / cantidad;
Console.WriteLine("lA media es: {0}", media);


Console.WriteLine("Los numeros mayores que la media son:");
for (int i = 0; i < cantidad; i++)
{
    if (numeros[i] > media)
    {
        Console.WriteLine(numeros[i]);
    }
}
