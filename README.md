# Zadania

## Ćwiczenie 1: Pierwszy workflow
**Cel:** Utwórz prosty workflow, który uruchamia się przy każdym pushu do repozytorium i wypisuje „Hello, GitHub Actions!” w logach.

**Wskazówki:**

- Użyj eventu push
- Job powinien działać na ubuntu-latest
- Użyj kroku run: echo "Hello, GitHub Actions!"

## Ćwiczenie 2: Workflow z warunkiem
**Cel:** Zmodyfikuj workflow tak, aby uruchamiał się tylko, gdy zmieniany jest plik w katalogu src/.

**Wskazówki:**

- Użyj paths w definicji eventu push

## Ćwiczenie 3: Automatyczne testy
**Cel:** Utwórz workflow, który uruchamia testy jednostkowe w Pythonie po każdym pushu.

**Wskazówki:**

- Użyj actions/setup-python
- Zainstaluj zależności z requirements.txt
- Uruchom pytest

##Ćwiczenie 4: Matrix build
**Cel:** Zbuduj workflow, który testuje aplikację na wielu wersjach Pythona (np. 3.8, 3.9, 3.10).

**Wskazówki:**

- Użyj strategy.matrix w definicji joba

## Ćwiczenie 5: Automatyczne tworzenie release
**Cel:** Utwórz workflow, który automatycznie tworzy release na GitHubie, gdy dodany zostanie tag v*.

**Wskazówki:**

- Event: push z filtrem na tags
- Użyj actions/create-release

## Ćwiczenie 6: Użycie secrets
**Cel:** Utwórz workflow, który używa sekretu (np. tokenu API) do wykonania zapytania HTTP.

**Wskazówki:**

- Dodaj sekret w ustawieniach repozytorium
- Użyj curl z secrets.MY_SECRET

## Ćwiczenie 7: Upload przez ftp
**Cel:** Utwórz workflow, który wystawia pliki z folderu **.dist/** przez ftp na serwer clienta

**Wskazówki:**

- Dodaj login, link do ftp oraz hasło przez sekret w github
- użyj 50min ftp do weryfikacji workflow
