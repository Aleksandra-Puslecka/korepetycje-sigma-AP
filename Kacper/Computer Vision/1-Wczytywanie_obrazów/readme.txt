# Powtórzenie z lekcji 2
## 1. Typy komórek w Jupyter Notebook
 Code - Komórki służące do pisania i wykonywania kodu.
 Markdown - Komórki do pisania tekstu.
## 2. Po co transformujemy obrazy?
#### 2.1. Augmentacja danych
Aby zwiększyć różnorodność danych treningowych w uczeniu maszynowym bez potrzeby zbierania nowych obrazów.
#### 2.2. Wyostrzenie elementów
W celu uwidocznienia kluczowych cech, takich jak krawędzie lub tekstury.
#### 2.3. Standaryzacja danych
Aby ujednolicić obrazy (rozmiar, wartości pikseli), co poprawia efektywność modeli.
#### 2.4. Poprawa czytelności 
Dla lepszej analizy przez ludzi lub algorytmy (np. redukcja szumu, poprawa kontrastu).
#### 2.5. Wzmacnianie ukrytych wzorców
Aby wydobyć informacje niewidoczne na pierwszy rzut oka, np. krawędzie.
#### 2.6. Zmiana przestrzeni kolorów
Dostosowanie obrazu do specyficznych potrzeb analizy, np. konwersja do odcieni szarości.

## 3. Jak komputer widzi obrazy?
#### Obrazy w kolorze RGB 
Każdy piksel obrazu ma trzy wartości (R, G, B – czerwony, zielony, niebieski).
#### Struktura danych 
Obrazy to macierze (listy w listach) w Pythonie.

###### pixel = [255, 0, 0]  # Czerwony piksel
###### image = [[[255, 0, 0], [0, 255, 0]], [[0, 0, 255], [255, 255, 255]]]
## 4. Indeksy w listach i slice-y (wycinki list)
patrz Python Essential/Listy_Tuple_Sety_Słowniki.ipynb
## 5. Floor division (//) i komentarze wielolinijkowe("""    """)
## 6. Czym różni się len() od shape?
len() -  Zwraca długość pierwszego wymiaru (np. liczba wierszy listy lub macierzy).
shape - Atrybut tablic numpy, zwraca pełne wymiary (np. (liczba wierszy, liczba kolumn)).

##### import numpy as np
##### array = np.array([[1, 2], [3, 4]])
##### print(len(array))      # Wynik: 2
##### print(array.shape)     # Wynik: (2, 2)
## 7. Funkcje pakietu OpenCV
imread(): Wczytuje obraz z pliku.
imshow(): Wyświetla obraz w osobnym oknie.
waitKey(): Zatrzymuje działanie programu, czekając na naciśnięcie klawisza.
## 8. Czym dokładnie jest waitKey()?
Opis: Funkcja czeka na naciśnięcie klawisza przez użytkownika.
Argument w waitKey() określa czas oczekiwania w milisekundach (0 → czeka w nieskończoność).
Przydatne przy wyświetlaniu obrazów, aby program nie zamykał okna natychmiast po jego otwarciu - inaczej kod się zatnie lub wyskoczy error bo obraz zamrożony. 

