#Rozwiązania C


Zadanie 1. Napisać i uruchomić program w C, który wczytuje liczbę naturalną "n" i drukuje wartości słowem kwadratów.
```c
main () {
  int n,suma,i;
  suma=0;
  printf ("Podaj liczbe n:\n");
  scanf("%i", &n);
  for (i=1 ; i<=n; i++) 
    suma=suma+i*i;
  printf("Wynik sumy to: %i\n" ,suma);
}
```

Zadanie 2. Napisać program obliczający wartość każdego z poniższych wyrażeń.
```c
main () {
  int n1,n2,n3;
  n1=5+3*8/2-3;
  printf("n1 wynosi: %i \n",n1);
  n2=2%2+2*2-2/2;
  printf("n2 wynosi: %i \n", n2);
  n3=2*4*(5+9/2);
  printf("n3 wynosi: %i \n", n3);
}
```

Zadanie 3. W miejsce kropek"..." wpisz kod tak, aby powstał działający program. Program wypisuje liczby z tablicy tabela
[], w odwrotnej kolejności, takiej jak 12,6,4,2,1.
```c
int main() {
int tabela[]={1,2,4,6,12};
 int a;
 for (a=4 ; a>=0; a=a-1)
   printf("%i \n", tabela[a]);
 return 0; 
}
```

Zadanie 4. Program wypisujący kolejne potęgi 2, nie przekraczające 2010. FOR.
```c
main () {
  int a=1;
  for (a=1; a<=2010; a=a*2)
    printf ("%i \n", a);
}
```

Zadanie 5. Program wypisujący kolejne potęgi 2, nie przekraczające 2010. WHILE.
```c
main () {
  int a;
  a=1;
  while ( a<=2010) {
   printf("%i\n",a);
   a=a*2;}

}
```

Zadanie 6. Program wyliczający coś tam.
```c
main() {
  int n,suma;
  n=1;
  suma=0;
  for(n=1; n<31; n=n+1){
    if{ (n<16)
  printf ("Aktualna liczba to:%i \n",n);
    
    else{ 
 printf("Aktualna liczba to:%i \n", n*2);
    }
    }
}
}
```

Zadanie 7. Program obliczający kwadrat i sześcian podanej liczby.
```c
main(){
  int i;
  printf("Podaj liczbe");
  scanf("%i", &i);
  printf("Kwadrat to: %i \n" , i*i);
  printf("Szescian to: %i \n", i*i*i);
}
```

Zadanie 8. Program przeliczajacy z systemu dziesiatkowego na binarny.
```c
main(){
int liczba=8;
int i;
int wynik[20];
printf("Podaj liczbę w systemie 10: ");
scanf("%i",&liczba);
i=0;
while(liczba!=0)
{
    wynik[i]=liczba%2;
    printf(" RESZTA %i przez 2 = %i ",liczba,wynik[i]);
    liczba=liczba/2;
    printf(" PO PODZIELENIU LICZBA =  %i \n", liczba);
    i++;
}
printf("\nWYNIK:");
for(i=i-1;i>=0;i--) printf(" %i ",wynik[i]);


}
```
