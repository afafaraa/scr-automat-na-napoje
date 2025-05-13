Aleksandra Fąfara | email: olafafara@student.agh.edu.pl

Uwaga! Ponkty oznaczone (?) są dodatkowymi pomysłami, które planuję zrealizować jeżeli wszystkie inne będą zrealizowane i wystarczy mi czasu.

# Automat do kawy obsługujący napoje 

## Opis systemu
Automat będzie miał do wyboru skończoną ilość napojów do zamówienia. Aby dokonać zakupu użytkonik musi najpierw wybrać napój, a następnie rodzaj płatności (kratą (?) lub gotówką).  Jeżeli napój nie jest dostępny pojawi się odpowiednie powiadomienie. W przypadku gotówki automat obsługuje wyłącznie monety o wartościach: 10gr, 20gr, 50gr, 1zł, 2zł, 5zł.

## Opis techniczny
1. Definicja komponentów systemu

    - Komponenty wykonawcze:

        Komponnet do obsługi żądań: Odpowiada za przyjmowanie zamówień od użytkowników. Najpierw należy wybrać napój, następnie jeżeli jest on dostępny (Sensor dostępności), to należy dokonać wyboru płatności. (Możliwe, że zostanie rozbity na 2 komponenty zaleźne od siebie.)

        Moduł płatności: Obsługuje transakcje płatnicze, w tym: liczenie monet i zatwierdzanie że suma się zgadza (Sensor płatności) oraz płatność kartą (?).

        Dozownik napojów: Element odpowiedzialne za wykonanie napojów.

        Kontroler główny: Odpowiada za zarządzanie całością procesu.

    - Komponenty sensoryczne:

        Sensor dostępności napoju: Monitoruje poziom zapasów napoju w maszynie.

        Sensor płatności: Potwierdza, że transakcja płatnicza została poprawnie zakończona.

2. Zarządzanie stanem
   - Automat będzie miał 3 stany: "czekanie na wybranie napoju" (stan domyślny), "czekanie na wybranie rodzaju płatności", "wydawanie napoju".

3. Bezpieczeństwo i zarządzanie błędami (?)
    - Reakcje na błędy: komponenty do obsługi awarii, mechanizmy odzyskiwania, np. powtarzanie płatności lub zwrot pieniędzy.





