# algoritmos#include "stdafx.h"
#include <iostream>
#include "conio.h"
#include "math.h"

using namespace std;
 
 int main ()
 {
	 int area, promedio, mayor, lado, n1, n2, n3, A, B, opcion;
	 do {
		 cout<< "********MENU******\n";
		 cout<< "1.- area del cuadrado\n";
		 cout<< "2.- promedio de tres numeros\n";
		 cout<< "3.- mayor de dos numeros\n";
		 cout<< "0.- salir\n";
		 cout<< "opcion: ";
		 cin>> opcion;

		 switch (opcion)
		 {
		 case 1:

		   cout<< "cuanto es el lado del cuadrado?";
		   cin>> lado;
		   area=lado*lado;
		   cout<< "el area del cuadrado es: "<<area;
		   break;

		 case 2:
		   cout<< "inserte el primer numero\n";
		   cin>> n1;
		   cout<< "inserte el segundo numero\n";
		   cin>> n2;
		   cout<< "inserte el tercer numero\n";
		   cin>> n3;
		   promedio = (n1+n2+n3)/3;
		   cout<< "el promedio de los numeros es: "<<promedio;
		   break;

		 case 3:   

			 cout<< "ingrese el primer numero";
			 cin>> A;
			 cout<< "ingrese el segundo numero";
			 cin>> B;
			 if (A>B) {
				 cout<< "el mayor es: "<<A;
			 }
			 cout<< "el mayor es: "<<B;
			 break;
         
		 case 0:

			 cout<< "salir";
			 break;

		 default:
			 cout<< "opcion invalida";
			 break;
		 }
		 getch ();
		 system("cls");
	 } while (opcion != 0);

	 return 0;
 } 

