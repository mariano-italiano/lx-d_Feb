# Stany kontenera:
- created: utworzony, gotowy do uruchomienia
- up - działający (wykonujący zadanie)
- exited - wyłączony, w trybie bezczynności (po zakończeniu zadania)
- paused - wstrzymany 
- restarting - w trakcie ponownego uruchamiania


# Proces uruchamiania kontenera: 
1. Pobranie image'a bazowego (pod warunkiem że nie ma go lokalnie).
2. Utworzenie kontenera.
3. Załadowanie systemu plików i utworzenie warstwy r/w (zapis/odczyt).
4. Zainicjowanie sieci (bridge network).
5. Konfiguracja sieci (adresu IP).
6. Uruchomienie kontenera.
7. Przechwytywanie wyjścia - utworzenie i prowadzenie logów.
