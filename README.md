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
Zadanie 9. Napisz program, ktory wczyta liczbę całkowitą i wypisze czy jest większa od 5.
```c
main () {
  int i;
  printf("Podaj liczbe calkowita\n");
  scanf("%i", &i);
  if ( i>5) 
    printf("Twoja liczba jest wieksza niz 5 \n");
    else printf("Twoja liczba jest mniejsza od 5 \n");
  
}
```
Zadanie 10. Napisz program, ktory wczyta liczbe calkowita i wypisze czy jest dodatnia, ujemna czy rowna 0.
```c
main () {
  int i;
  printf("Podaj liczbe calkowita\n");
  scanf("%i", &i);
  if (i>0)
    printf("Twoja liczba jest dodatnia\n");
  else if (i<0)
 printf("Twoja liczba jest ujemna\n");
  else 
    printf("Twoja liczba jest rowna zero\n");
  }
```
Zadanie 11. Napisz program, ktory wczyta liczbe calkowita i wypisze czy jest parzysta czy nieparzysta.
```c
main () {
  int i;
  printf("Podaj liczbe calkowita:\n");
  scanf("%i", &i);
  if (i%2)
    printf("Twoja liczba jest nieparzysta\n");
  else printf("Twoja liczba jest parzysta\n");
}
```
Zadanie 12. Napisz program, ktory wczyta dwie liczby calkowite i wypisze czy sa rowne.
```c
main () {
  int i,j;
  printf("Podaj pierwsza liczbe\n");
  scanf("%i", &i);
  printf("Podaj druga liczbe\n");
  scanf("%i", &j);
  if (i==j)
    printf("Twoje liczby sa rowne\n");
  else 
    printf("Twoje liczby nie sa rowne\n");
}
```
Zadanie 13. Napisz program, ktory wczyta 2 liczby calkowite i wypisze ktora z nich jest wieksza.
```c
main () {
  int i,j;
  printf("Podaj pierwsza liczbe\n");
  scanf("%i", &i);
  printf("Podaj druga liczbe\n");
  scanf("%i", &j);
  if(i>j)
    printf("Pierwsza liczba jest wieksza od drugiej\n");
  else
    printf("Druga liczba jest wieksza od pierwszej\n");
}
```
Zadanie 14. Napisz program, ktory obliczy i wypisze na ekran sume kwadratow liczb od 1 do 20.
```c
main () {
  int suma,i;
  suma=0;
  for (i=1; i<=20; i++)
  suma=suma+i*i;
  printf("Wynik sumy dwudziestu kwadratow to: %i\n" , suma);
}
```
Zadanie 15. Napisz program, ktory wczytuje liczbe calkowita n>=0, a nastepnie n liczb rzeczywistych (double %lf) i drukuje
te liczby w trzech kolumnach w taki sposob, zeby zachowac krycie (tzn. kropka dziesietna zawsze byla w tych samych kolumnach)
Np gdy uzytkownik poda 7  0,12  -31.5 2.5 -59,01
                      26.4  -12.0 8.3
                      
Kol1.     Kol2.     Kol3.
0,12      -31.50    2.50
-59.01    26.40     -12.00
8.30      
Mozna zakladac, ze liczby naleza do przedzialu (-100; 100)
(Zeby wydrukowal l. rzeczywiste na polu o dl 6 znakow z 2 cyframi po kropce nalezy w komendzie printf uzyc formatu
"%6.2lf)
```c
main () {
  int n,i;
  printf("Podaj n\n"); 
  scanf("%i\n", &n);
  /*deklarowanie tablicy*/
  double tab[n];
  /*petla wczytujaca dane do tablicy*/
  for (i=0 ; i<n ; i++)
    scanf("%lf\n", &tab[i]);
  /*petla wypisujaca dane z tablcy*/
  for (i=0 ; i<n ; i++) {
    printf("%2.2lf\n", tab[i]);
    if (i%3==2)
      printf("\n");
  }
}
```
Zadanie 16. Napisz program ktory wczyta od uzytkownia dane do piecioelementowej tablicy liczb calkowitych, a nastepnie 
wypisze na ekran sume jej elementow.
```c
main () {
  int i,j,suma;
  //nadawanie poczatkowej wartosci zmiennej suma
  suma=0;
  //wczytywanie ilosci liczb
  printf("Podaj liczbe\n");
  scanf("%i", &j);
  //deklaracja tablicy
  int tab[j];
  //wczytywanie liczb do tablicy
  for (i=0 ; i<j ; i++)
    scanf("%i", &tab[i]);
  //wyliczanie wartosci sumy
  for (i=0; i<j; i++){
    /* printf("%i\n", tab[i]);*/
  suma=suma+tab[i];
  }
  //wyswietlanie wyniku
  printf("Wynik to %i \n ", suma);
}
```
Zadanie 17. Napisz program ktory wczyta od uzytkownika dane do piecioelementowej tablicy liczb calkowitych, a nastepnie
przestawu jej pierwszy element z ostatnim i wypisze cala tablice na ekran.
```c

