﻿# PIO_CROSSY_ROAD

**Tytuł:** Pass the exam.

**Liczba graczy:** 3

**Info:** Gra typu Crossy road (https://en.wikipedia.org/wiki/Crossy_Road), jednak w 2D.

**Przebieg gry:** Gracze zaczynają od startu po lewej stronie ekranu i kierują się w prawą stronę – w stronę mety. Po drodze muszą unikać różnych przeszkód, część z nich powoduje automatyczną przegraną. Gracze kolidują ze sobą, tj. nie mogą na siebie wchodzić, przez co mogą sobie przeszkadzać. Gra kończy się w momencie, kiedy pierwszy gracz dotrze na metę.

**Warunek zwycięstwa:** Gracz jako pierwszy dociera do mety. 

**Warunek przegranej:** Gracz wchodzi w kolizje z przeszkodą, która powoduje automatyczną przegraną lub nie dotarcie do mety w momencie, kiedy inny gracz do niej dotarł lub pierwszy gracz ma zbyt dużą przewagę względem gracza ostatniego, wtedy ostatni gracz przegrywa.

**Warunek braku zwycięzcy:**  Każdy z graczy przegrał przed dotarciem do mety.

# Środowisko

Do działania potrzebny jest python 3.10.11.

Potrzebne biblioteki można zainstalować poprzez odpalenie cmd w głównym folderze gry i wpisanie komendy:

pip install -r requirements.txt

# Uruchomienie gry

Na początku uruchamiamy server.py. Następnie możemy uruchomić client.py. Żeby gra została uruchomiona, potrzebne są 3 osoby w lobby, dlatego client musi być odpalony 3 razy.

Uwaga! W server i client trzeba zmienić IP na to, na które chcemy się podłączyć. server.py: SERVER_IP, client.py: HOST_IP

# 1 sposób - w terminalu
Do uruchomienia każdego z programów potrzebujemy oddzielnie uruchomione terminale (1 dla serwera, 3 dla graczy).
Upewniamy się, że terminal CMD ustawiony jest na folderze z grą. 
Serwer uruchamiamy poprzez komendę "python server.py". Gracza uruchamimay przez komendę "python client.py".

# 2 sposób - w pełni w Pycharmie

- server.py
server.py uruchamiamy jak normalny program w Pycharmie.

- client.py
W celu możliwości uruchomienia trzykrotnie client.py musimy wykonać następujące kroki:
1. Wchodzimy w "Edit Configurations..." (znajduje się to w rozwijanej liście, kiedy klikniemy na nazwę programu, który chcemy uruchomić obok przycisków do uruchomienia czy debugowania.)
2. Zaznaczamy opcję "Allow parallel run".
3. Zatwierdzamy "Apply".
4. Uruchamiamy 3 razy jak normalny program.
