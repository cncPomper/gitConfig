# Najprzydatniejsze komendy gita z których korzystam, ich zastosowanie i parę innych przydatnych tricków:)

 ## 1. Konfiguracja środowiska
 ### 1.1 Kim jesteś?
 ```
 git config --global user.name "Imię Nazwisko"
 ```
 ```
 git config --global user.email moj@email.com
 ```

## 2. Narzędzia
 -> Autohotkey - przyspiesza pracę oraz pozwala unikać błędów [AutoHotKey](https://www.autohotkey.com/)
 <br/>
 -> gitk - jest instalowany w czasie instalowania gita

## 3. Tworzenie historii
### 3.1 Dodanie zmian w pliku/plikach i ich zapisanie
Można dodać/skomitować wszystkie nowe zmiany poprzez użycie następujących komend
```
git add .
```
```
git commit -m "COMMIT MESSAGE"
```
### 3.2 Świadome dodawanie zmian
Minus poprzedniego rozwiązania jest taki, że musimy pamiętać o tym żeby komitować na bieżąco zmiany. W tym sposobie nawet jeśli zrobimy wiele zmian w wielu miejscach możemy to łatwo rozdzielić na komity
```
git add -p
```
Ta komenda wyświetla w bashu zmiany dla danych plików w sposób rozbity. Dzieli zmiany na czytelne 'patche' które użytkownik może łączyć w większe komity.
->
<br/>
->
<br/>
->

## 4. Integracja z github.com i wysyłanie zmian
## 5. Pobieranie zmian
Najbezpieczniej jest zamiast klasycznie
```
git pull
```
Najpierw użyć komendy fetch
```
git fetch
```
Wtedy nie mergujemy jeszcze naszego lokalnego mastera z pobranymi zmianami tylko pobierami same zmiany bez integracji ich z naszym lokalnym środowiskiem.
