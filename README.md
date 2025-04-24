# Codigo_Prueba
#include <iostream>
using namespace std;

int main (){
    //VARIABLES
    char nombre[20],apellido[20],direccion[50],correo[30],prod1[20],prod2[20],prod3[20];
    int opcion=0,id;
    float p1=0,p2=0,p3=0,subtotal,iva,total;

while(opcion!=4){

cout<<"MENU"<<endl;
cout<<"1. Datos del cliente"<<endl;
cout<<"2. Ingreso de productos"<<endl;
cout<<"3. Calculo de factura"<<endl;
cout<<"4. Salir"<<endl;

cout<<"Seleccione una opcion: ";
cin>>opcion;

switch(opcion){

case 1:{
    cout<<"Escriba el nombre y apellido del cliente: "<<endl;
    cin>>nombre;
    cin>>apellido;
    cout<<"Ingrese su cedula: "<<endl;
    cin>>id;
    cout<<"Ingrese su correo: "<<endl;
    cin>>correo;
    cout<<"Ingrese su direccion: "<<endl;
    cin>>direccion;
    break;
    }

case 2:{
    cout<<"Registraremos sus productos: ";
    cout<<"Por favor, indique su primer producto: ";
    cin>>prod1;
    cout<<"Ingrese el precio del producto: ";
    cin>>p1;

    cout<<"Por favor, indique su segundo producto: ";
    cin>>prod2;
    cout<<"Ingrese el precio del producto: ";
    cin>>p2;

    cout<<"Por favor, indique su tercer producto: ";
    cin>>prod3;
    cout<<"Ingrese el precio del producto: ";
    cin>>p3;
    break;
    }

case 3: {
    subtotal=p1+p2+p3;
    iva=subtotal*0.15;
    total=iva+subtotal;
    cout<<"FACTURA"<<endl;
    cout<<"CLIENTE: "<<nombre<<" "<<apellido<<endl;
    cout<<"CEDULA: "<<id<<endl;
    cout<<"CORREO: "<<correo<<endl;
    cout<<"DIRECCION: "<<direccion<<endl;
    cout<<"El subtotal de su compra es: $"<<subtotal<<endl;
    cout<<"IVA: $"<<iva<<endl;
    cout<<"El total a pagar es de: $"<<total<<endl;
    break;
    }

case 4: {
    cout<<"GRACIAS POR SU COMPRA!"<<endl;
    break;
    }

    default: {
    cout<<"OPCION INVALIDA. INTENTE DE NUEVO."<<endl;
    }

}
}
return 0;
}
