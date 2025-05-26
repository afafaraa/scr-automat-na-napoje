Aleksandra Fąfara | email: olafafara@student.agh.edu.pl

# Automat do kawy obsługujący napoje 

## Opis systemu
Automat będzie miał do wyboru skończoną ilość napojów do zamówienia. Aby dokonać zakupu użytkonik musi wybrać napój wyświetlonych na ekranie. Jeżeli napój nie jest dostępny pojawi się odpowiednie powiadomienie. W przeciwnym przypadku automat czeka na płatność i po potwierdzeniu jej zwraca napój. Automat obsługuje wyłącznie monety o wartościach: 10gr, 20gr, 50gr, 1zł, 2zł, 5zł.

## Opis techniczny
1. Definicja komponentów systemu

    - Komponenty wykonawcze:

        Komponnet do obsługi żądań (Request_Handler): Odpowiada za przyjmowanie zamówień od użytkowników oraz zwracania użytkownikowi informacji o stanie automatu.

        Moduł płatności (Payment_Module): Obsługuje transakcje płatnicze, w tym: liczenie monet i zatwierdzanie że suma się zgadza (Sensor płatności).

        Dozownik napojów (Drink_Dispenser): Element odpowiedzialne za wykonanie napojów oraz sprawdzanie czy napój jest dostępny (Sensor dostępności napoju).

    - Komponenty sensoryczne:

        Sensor dostępności napoju (Drink_Availability_Sensor): Monitoruje poziom zapasów napoju w maszynie.

        Sensor płatności (Payment_Sensor): Potwierdza, że transakcja płatnicza została poprawnie zakończona.

2. Zarządzanie stanem
   - Automat będzie miał następujące stany: "IDLE", "DRINK_SELECTED", "WAITING_FOR_PAYMENT", "PAYMENT_RECEIVED", "MAKING_DRINK", "DRINK_READY".

