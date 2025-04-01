# api-cli-fetcher


## Opis projektu
Aplikacja CLI, która pobiera dane z API i zapisuje je do pliku JSON.

## Instalacja
1. **Pobierz repozytorium**:
   ```sh
   git clone https://github.com/lukaszmazur0105/api-cli-fetcher.git
   cd api-cli-fetcher
   ```
2. **Zainstaluj wymagane zależności**:
   - Dla Pythona:
     ```sh
     pip install -r requirements.txt
     ```
   - Dla Node.js:
     ```sh
     npm install
     ```

## Uruchomienie aplikacji
Uruchomienie aplikacji z podstawową komendą:
   ```sh
   ./cli_fetcher --fetch --url https://api.example.com/data
   ```
Dane zostaną zapisane do `output.json`

## Przykłady komend
- Pobranie danych z API:
  ```sh
  ./cli_fetcher --fetch --url https://api.example.com/data
  ```
- Zmiana nazwy pliku wyjściowego:
  ```sh
  ./cli_fetcher --fetch --url https://api.example.com/data --output data.json
  ```

## Rozszerzalność
Aby dodać nowe źródła danych:
1. Dodaj nowy endpoint do konfiguracji w `config.json`.
2. Zaimplementuj funkcję obsługującą nowy typ danych w `fetcher.py` lub `fetcher.js`.
3. Uruchom ponownie aplikację z odpowiednimi parametrami.
