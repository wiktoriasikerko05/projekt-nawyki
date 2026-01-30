HabitFlow - System Monitorowania Nawyków


**HabitFlow** to aplikacja typu PWA/SPA (Single Page Application) służąca do śledzenia postępów w budowaniu nawyków. Projekt kładzie nacisk na grywalizację (Gamification), wizualizację danych w czasie rzeczywistym oraz pełną prywatność użytkownika (Local-First Architecture).

---

Kluczowe Funkcjonalności

Aplikacja została zaprojektowana z myślą o skalowalności i wygodzie użytkowania ("Enterprise Ready").

### 1. Zarządzanie Danymi (Data Management)
* **System Importu/Eksportu:** Pełna obsługa serializacji danych do formatu `.json`. Użytkownik może wykonać backup swoich postępów (Eksport) oraz przywrócić go na innym urządzeniu (Import) z walidacją poprawności pliku.
* **Local Persistence:** Wykorzystanie `LocalStorage API` do trwałego przechowywania stanu aplikacji po stronie klienta (brak konieczności połączenia z serwerem).

### 2. Algorytmika i Logika Biznesowa
* **Smart Streak Algorithm:** Autorski algorytm obliczania ciągłości serii (Streak). System analizuje historię dat, sortuje je chronologicznie i wylicza nieprzerwany ciąg dni, ignorując luki czasowe wynikające ze stref czasowych.
* **Grywalizacja (Gamification):** System nagród wizualnych. Po osiągnięciu cyklicznych celów (np. co 7 dni serii), silnik cząsteczkowy generuje animację fajerwerków (Particle System) w Canvas/DOM.

### 3. Interfejs i UX (User Experience)
* **Theme Switcher:** Dynamiczne przełączanie motywu (Jasny/Ciemny) oparte na zmiennych CSS (`:root` variables).
* **Global Dashboard:** Kołowy wykres postępu (Conic Gradient) pokazujący dzienną produktywność w czasie rzeczywistym.

---

Stack Technologiczny

* **Core:** JavaScript (ES6+) - wykorzystanie `Arrow Functions`, `Array Methods` (map, filter, reduce, sort), `Blob API` (do eksportu plików) oraz `FileReader API` (do importu).
* **UI/Styling:** CSS3, Flexbox, CSS Grid, CSS Transitions, CSS Variables (do obsługi motywów).
* **Storage:** Web Storage API (LocalStorage).

---

Instalacja i Uruchomienie

Aplikacja jest statyczna i nie wymaga środowiska uruchomieniowego typu Node.js.

1.  **Pobranie repozytorium:**
    ```bash
    git clone [https://github.com/wiktoriasikerko05/projekt-nawyki.git]
    ```
2.  **Uruchomienie:**
    Otwórz plik `index.html` w dowolnej nowoczesnej przeglądarce (Chrome, Firefox, Edge, Safari).

