# APBD Cw 1 
 zad 5
Merge nie byˆ fast-forward bo galaz main poszla do "przodu" przez commit z README przed wykonaniem mergea 

odp na 3 pytania:
1. Kiedy Git wykona fast-forward, a kiedy powstaje merge commit?

Fast-forward wykona sie gdy ga³¹Ÿ nie otrzymuje nowych commitow od momentu stworzenia nowej bocznej ga³êzi.
Git przesuwa wskaznik ga³êzi main na ostatni commit z bocznej ga³êzi

Merge commit mamy gdy ga³êzie siê rozga³êzi³y, czyli mamy dwa rozne commity na ga³êzi main i na ga³êzi bocznej.
Tworzony jest wtedy dodatkowy commit, który ³¹czy te dwie œcie¿ki

2. Czym w praktyce ró¿ni siê merge od rebase? 

Merge zapisuje realn¹ historie pracy, widaæ gdzie ga³êzie siê rozdwajaj¹ i zaczynaj¹

Rebase tutaj historia jest przepisywana i wygl¹da jak jedna prosta linia poniewa¿ commity z bocznych ga³êzi s¹ przenoszone na aktualny main

3. W jaki sposób zosta³ rozwi¹zany konflikt w Twoim repozytorium?

Najpierw zmodyfikowa³am t¹ sam¹ liniê kodu w Program.cs. Po otworzeniu pliku zamieni³am 

```csharp
<<<<<<< HEAD
Console.WriteLine("Wersja main");
=======
Console.WriteLine("Wersja feature-conflict");
>>>>>>> feature-conflict

na po³¹czenie 2 komunikatow w 1 komunikat. Uzy³am komendy git add i zakonczylam commitem

