#include <iostream>
#include <stdlib.h>
#include <time.h>
using namespace std;
void jugar(int vector[], int t);
void llenarVe2(int vector[], int tamaño);
void ganador(int p1, int p2);
int dado();
int main(){
    int vector[100]={0}, tamaño=100;
    cout << "Serpientes y escaleras!\n";
    srand(int(time(NULL)));
   llenarVe2 (vector, tamaño);
    jugar (vector, tamaño);

    return 0;
}
void jugar(int vector[], int t){
    int p1 = 0, p2=0;
    while(p1<t && p2<t)
    {
        p1 += dado();

        if (p1<t){
            if (vector[p1]>0)
                cout<<p1<<"jugador #1 escalera\n";
            else if (vector[p1]<0)
                cout<<"Serpiente\n";
            p1 += vector[p1];
            cout<<"el jugador 1 se encuentra en la posicion:"<<p1<<"\n";
        }
        
        p2 += dado();
        if (p2<t) {
            if (vector[p2]>0)
                cout<<p2<<"jugador #2 escalera\n";
            else if (vector[p2]<0)
                cout<<"Serpiente\n";
            p2 += vector[p2];
            cout<<"el jugador 2 se encuentra en la posicion:"<<p2<<"\n";
        }
    }
    
    if (p1>p2)
        cout<<" Win el jugador #1 \n";
    else
        cout<<" Win el jugador #2 \n";
}
int dado()
{
    int numeroAleatorio;
    return numeroAleatorio = 1+rand()%6;
}
void llenarVe2(int vector[], int tamaño)
{
    vector[3]= +6;
    vector[7]=  +5;
    vector[15]= +9;
    vector[20]= +9;
    vector[40]= +6;
    vector[54]= +9;
    vector[47]= +3;
    vector[83]= +9;
    vector[32]= +11;
    vector[47]= +10;
    
    vector[50]= -2;
    vector[40]= -6;
    vector[90]= -8;
    vector[65]= -7;
    vector[76]= -8;
    vector[34]= -16;
    vector[80]= -9;
    vector[6]= -3;
    vector[20]= -10;
    vector[82]= -8;
}
