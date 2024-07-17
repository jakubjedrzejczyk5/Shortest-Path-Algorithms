# Shortest-Path-Algorithms
# Algorytmy Najkrótszej Ścieżki

## Opis Projektu

Projekt ten obejmuje implementację i wizualizację dwóch algorytmów znajdowania najkrótszej ścieżki w grafach skierowanych: algorytmu Dijkstry oraz algorytmu Bellmana-Forda. 

## Implementowane Algorytmy

### Algorytm Dijkstry
- **Opis**: Algorytm Dijkstry znajduje najkrótszą ścieżkę od wierzchołka początkowego do wszystkich pozostałych wierzchołków w grafie z wagami nieujemnymi.
- **Szczegóły Implementacji**: 
  - Inicjalizacja odległości wszystkich wierzchołków jako nieskończoność, z wyjątkiem wierzchołka startowego (odległość 0).
  - Użycie kolejki priorytetowej do wybierania wierzchołka z najmniejszą znaną odległością.
  - Aktualizacja odległości sąsiadujących wierzchołków, jeśli możliwe jest znalezienie krótszej ścieżki.

### Algorytm Bellmana-Forda
- **Opis**: Algorytm Bellmana-Forda znajduje najkrótszą ścieżkę od jednego wierzchołka do wszystkich innych w grafie, nawet jeśli krawędzie mają wagi ujemne. Może również wykrywać cykle o ujemnej wadze.
- **Szczegóły Implementacji**: 
  - Inicjalizacja odległości wszystkich wierzchołków jako nieskończoność, z wyjątkiem wierzchołka startowego (odległość 0).
  - Relaksowanie wszystkich krawędzi n-1 razy (gdzie n to liczba wierzchołków).
  - Sprawdzanie, czy istnieje cykl o ujemnej wadze po zakończeniu relaksacji krawędzi.
