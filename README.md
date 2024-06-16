# Specyfikacja Aplikacji OmniSync

## 1. Charakterystyka Oprogramowania

### 1.1 Nazwa Skrócona

OmniSync

### 1.2 Nazwa Pełna

OmniSync - System synchronizacji produktów eCommerce

### 1.3 Krótki Opis z Wskazaniem Celów

OmniSync jest zaawansowaną platformą przeznaczoną do dwukierunkowej synchronizacji produktów między różnymi sklepami internetowymi oraz centralnym systemem zarządzania. Celem platformy jest automatyzacja i usprawnienie procesów zarządzania produktami oraz klientami poprzez ich centralizację, co pozwala na oszczędność czasu, zwiększenie dokładności danych i lepsze zarządzanie zapasami. Wersja MVP skupia się na wspieraniu integracji z WooCommerce i Shopify, planowane są jednak rozszerzenia, które umożliwią współpracę z dodatkowymi platformami eCommerce.

## 2. Prawa Autorskie

### 2.1 Autor

KamilBuksa

### 2.2 Warunki Licencyjne

Oprogramowanie OmniSync jest wydane na licencji MIT. Licencja ta pozwala na bezpłatne używanie, modyfikację oraz dystrybucję oprogramowania, zarówno w formie pierwotnej, jak i zmodyfikowanej, pod warunkiem zachowania informacji o prawach autorskich i tekstu licencji. Licencja MIT jest jedną z najbardziej liberalnych licencji, co sprzyja szerokiemu rozpowszechnianiu i adaptacji oprogramowania, jednocześnie oferując ochronę praw autorskich twórców.

## 3. Specyfikacja Wymagań

### 3.1 Typy Użytkowników i Ich Role

#### Administrator

**Rola**: Administrator systemu odpowiada za ogólne zarządzanie systemem, w tym bezpieczeństwo, monitorowanie działania oraz zarządzanie kontami użytkowników.
**Odpowiedzialności**:

- Wysyłanie linków weryfikacyjnych do nowych użytkowników.
- Pełen dostęp do bazy danych produktów, umożliwiający zarządzanie i kontrolę nad wszystkimi wpisami.
- Zarządzanie kontami użytkowników, w tym blokowanie i odblokowywanie dostępu.
- Monitorowanie zdrowia systemu i reagowanie na incydenty.
- Aktualizacje systemu oraz zarządzanie patchami bezpieczeństwa.

#### Użytkownik OmniSync (Właściciel sklepu)

**Rola**: Właściciel sklepu korzysta z systemu do zarządzania produktami oraz integracjami z różnymi platformami eCommerce.
**Odpowiedzialności**:

- Rejestracja i weryfikacja konta przez e-mail.
- Logowanie z opcją dwuetapowej weryfikacji dla dodatkowego bezpieczeństwa.
- Dodawanie, konfiguracja i zarządzanie integracjami z platformami eCommerce.
- Zarządzanie produktami, w tym dodawanie, edytowanie i usuwanie produktów.
- Śledzenie i analizowanie danych dotyczących sprzedaży i zapasów.

### 3.2 Opis Grup Funkcjonalności

#### Zarządzanie Uprawnieniami i Użytkownikami

**Opis**: Funkcje umożliwiające administratorowi zarządzanie dostępem do systemu oraz kontrolę nad kontami użytkowników.
**Cechy**:

- Wysyłanie e-maili weryfikacyjnych do nowych użytkowników.
- Blokowanie i odblokowywanie użytkowników.
- Przeglądanie aktywności i logów użytkowników.
- Zarządzanie rolami użytkowników.

#### Integracje z Platformami eCommerce

**Opis**: Funkcje umożliwiające właścicielom sklepów dodawanie, konfigurację oraz zarządzanie integracjami z różnymi platformami sprzedaży online.
**Cechy**:

- Konfiguracja i zarządzanie integracjami (np. WooCommerce, Shopify).
- Monitoring stanu i zdrowia integracji.
- Synchronizacja danych produktów i klientów między platformami.

#### Zarządzanie Produktami

**Opis**: Funkcjonalność umożliwiająca użytkownikom OmniSync zarządzanie ich asortymentem produktów w różnych sklepach internetowych poprzez jednolity system.
**Cechy**:

- Dodawanie, edytowanie i usuwanie produktów.
- Zarządzanie kategoriami i atrybutami produktów.
- Automatyczna synchronizacja stanów magazynowych i cen między platformami.

#### Monitoring i Raportowanie

**Opis**: Funkcje zapewniające użytkownikom dostęp do danych analiz i raportów, które pomagają w podejmowaniu decyzji biznesowych.

**Cechy**:

- Generowanie raportów sprzedaży i analiz rynkowych.
- Śledzenie wydajności integracji i efektywności operacji sprzedażowych.lo

### 3.3 Historyjki Użytkownika

#### 3.3.1 Administrator

1. **Blokowanie Konta Użytkownika**

   - **Opis**: Jako Administrator, chciałbym mieć możliwość blokowania kont użytkowników, którzy naruszają zasady korzystania z systemu, aby zapewnić bezpieczeństwo i prawidłowe funkcjonowanie platformy.
   - **Priorytet**: 1 - wymagane

2. **Odblokowywanie Konta Użytkownika**

   - **Opis**: Jako Administrator, chciałbym mieć możliwość odblokowywania kont użytkowników, aby umożliwić im ponowne korzystanie z systemu po rozwiązaniu problemów prawnych lub technicznych.
   - **Priorytet**: 1 - wymagane

3. **Monitorowanie Aktywności Użytkowników**
   - **Opis**: Jako Administrator, chciałbym mieć dostęp do logów aktywności wszystkich użytkowników, aby móc analizować ich działania i reagować na ewentualne anomalie.
   - **Priorytet**: 2 - przydatne

#### 3.3.2 Właściciel Sklepu

1. **Dodawanie Integracji z Platformą eCommerce**

   - **Opis**: Jako Właściciel Sklepu, chciałbym móc łatwo dodawać integracje z różnymi platformami eCommerce, takimi jak WooCommerce i Shopify, aby rozszerzać moją działalność na nowe rynki i kanały sprzedaży.
   - **Priorytet**: 1 - wymagane

2. **Konfiguracja Integracji**

   - **Opis**: Jako Właściciel Sklepu, chciałbym mieć możliwość konfiguracji ustawień integracji, takich jak częstotliwość synchronizacji danych, aby dostosować procesy biznesowe do moich potrzeb.
   - **Priorytet**: 1 - wymagane

3. **Zarządzanie Produktami**

   - **Opis**: Jako Właściciel Sklepu, chciałbym mieć możliwość dodawania, edytowania i usuwania produktów w moim sklepie, aby aktualizować i zarządzać moim asortymentem zgodnie z potrzebami rynku.
   - **Priorytet**: 1 - wymagane

4. **Synchronizacja Stanów Magazynowych**

   - **Opis**: Jako Właściciel Sklepu, chciałbym, aby system automatycznie synchronizował stany magazynowe między różnymi platformami, aby uniknąć błędów wynikających z różnic w danych.
   - **Priorytet**: 1 - wymagane

5. **Generowanie Raportów Sprzedaży**

   - **Opis**: Jako Właściciel Sklepu, chciałbym generować szczegółowe raporty sprzedaży, aby analizować wyniki i optymalizować moje strategie biznesowe.
   - **Priorytet**: 2 - przydatne

6. **Zakup Subskrypcji**

- **Opis**: Jako Właściciel Sklepu, chcę mieć możliwość zakupu subskrypcji, która pozwoli mi na dodawanie produktów oraz integracji z platformami eCommerce, aby dostosować możliwości mojego sklepu do aktualnych potrzeb i strategii biznesowej.
- **Priorytet**: 1 - wymagane

### 3.4 Priorytety

Każda z historyjek użytkowników została przypisana do jednego z trzech poziomów priorytetów:

- **1 - Wymagane**: Krytyczne dla podstawowej funkcjonalności i operacji systemu.
- **2 - Przydatne**: Ulepszają doświadczenia użytkownika i efektywność operacyjną, ale nie są krytyczne.
- **3 - Opcjonalne**: Mogą być dodane później, aby rozszerzyć funkcjonalność systemu.

### 3.5 Moduł Subskrypcji

#### Typy Subskrypcji

1. **Pakiet Podstawowy**

   - **Cena**: 100 zł miesięcznie
   - **Ograniczenia**: Do 1000 produktów i 2 integracje
   - **Opis**: Idealny dla mniejszych przedsiębiorstw potrzebujących podstawowej funkcjonalności zarządzania niewielką liczbą produktów oraz integracji z dwiema platformami eCommerce.

2. **Pakiet Rozszerzony**

   - **Cena**: 250 zł miesięcznie
   - **Ograniczenia**: Do 10 000 produktów i 4 integracje
   - **Opis**: Skierowany do średnich sklepów, które poszukują rozszerzonej funkcjonalności oraz możliwości zarządzania większą liczbą produktów i integracji.

3. **Pakiet Premium**

   - **Cena**: 500 zł miesięcznie
   - **Ograniczenia**: Do 50 000 produktów i 6 integracji
   - **Opis**: Przeznaczony dla dużych sklepów z potrzebą obsługi dużej liczby produktów i wielu integracji, zapewniając kompleksowe zarządzanie zasobami.

4. **Pakiet Nieograniczony**
   - **Cena**: 1000 zł miesięcznie
   - **Ograniczenia**: Nieograniczona liczba produktów i integracji
   - **Opis**: Dla sklepów, które wymagają pełnej elastyczności i skalowalności bez jakichkolwiek ograniczeń w liczbie produktów czy integracji.

## 4. Testy

Testowanie jest niezbędnym elementem procesu weryfikacji aplikacji, zapewniając, że spełnia ona wymagania użytkowników i jest wolna od błędów. Dokładne scenariusze testów powinny obejmować wszystkie zdefiniowane funkcjonalności i historyjki użytkownika.

### 4.1 Plan Testów

Plan testów musi zawierać różne rodzaje testów, aby dokładnie sprawdzić każdą funkcję systemu:

- **Testy Jednostkowe**: Testy sprawdzające pojedyncze funkcje i metody w izolacji od reszty systemu.
- **Testy Integracyjne**: Weryfikacja, czy różne moduły i usługi współpracują ze sobą zgodnie z oczekiwaniami.
- **Testy Akceptacyjne**: Skupione na weryfikacji, czy system spełnia biznesowe wymagania.
- **Testy Wydajnościowe**: Zapewnienie, że system działa szybko i efektywnie podczas dużej liczby operacji.
- **Testy Bezpieczeństwa**: Identyfikacja i minimalizacja potencjalnych luk w zabezpieczeniach.

### 4.2 Scenariusze Testów

Scenariusze testowe powinny być bezpośrednio związane z poszczególnymi historyjkami użytkownika oraz ich priorytetami.

#### Scenariusze dla Administratora:

1. **Testowanie Blokowania Konta Użytkownika**

   - **Cel**: Sprawdzenie, czy mechanizm blokowania konta użytkownika funkcjonuje prawidłowo i jest w stanie efektywnie ograniczać dostęp do systemu.
   - **Kroki**:
     1. Administrator wybiera użytkownika do zablokowania.
     2. Administrator wybiera opcję blokady konta.
     3. System zapisuje zmianę statusu i uniemożliwia zablokowanemu użytkownikowi dostęp.
   - **Oczekiwany wynik**: Użytkownik jest skutecznie zablokowany, nie może logować się ani korzystać z systemu.

2. **Testowanie Odblokowywania Konta Użytkownika**
   - **Cel**: Weryfikacja, czy system prawidłowo przywraca dostęp do konta po jego odblokowaniu.
   - **Kroki**:
     1. Administrator wybiera użytkownika do odblokowania.
     2. Administrator wybiera opcję odblokowania konta.
     3. System zapisuje zmianę statusu i przywraca użytkownikowi dostęp do systemu.
   - **Oczekiwany wynik**: Użytkownik ma ponownie dostęp do swojego konta i wszystkich funkcji systemu.

#### Scenariusze dla Właściciela Sklepu:

1. **Testowanie Dodawania Integracji z Platformą eCommerce**

   - **Cel**: Sprawdzenie, czy właściciel sklepu może efektywnie dodać nową integrację z platformą eCommerce.
   - **Kroki**:
     1. Właściciel sklepu otwiera panel zarządzania integracjami.
     2. Właściciel wybiera opcję dodania nowej integracji.
     3. Właściciel konfiguruje i zapisuje ustawienia integracji.
   - **Oczekiwany wynik**: Nowa integracja jest dodana i prawidłowo skonfigurowana w systemie.

2. **Testowanie Synchronizacji Stanów Magazynowych**
   - **Cel**: Weryfikacja, czy informacje o stanie magazynowym są synchronizowane między różnymi platformami zgodnie z konfiguracją.
   - **Kroki**:
     1. Właściciel sklepu inicjuje proces synchronizacji.
     2. System przetwarza i aktualizuje stany magazynowe w zależności od ustawień.
   - **Oczekiwany wynik**: Stany magazynowe na różnych platformach są aktualne i spójne.

### 4.3 Sprawozdanie z Wykonania Scenariuszy Testów

Po przeprowadzeniu testów, wyniki powinny być dokładnie dokumentowane, włączając opis wykonanych działań, wykrytych błędów oraz sugerowane zmiany, które mogą poprawić funkcjonowanie systemu. Sprawozdanie to stanowi kluczowy element w procesie ciągłego doskonalenia oprogramowania.

## 5. Architektura Systemu

### 5.1 Opis Architektury Ogólnej

OmniSync składa się z dwóch głównych komponentów: backendu i frontend. Architektura systemu jest zaprojektowana w sposób modułowy, aby umożliwić łatwe rozszerzanie i utrzymanie aplikacji.

- **Backend**:

  - **Technologie**: Node.js, Nest.js
  - **Moduły**:
    - **AuthModule**: Zarządzanie autoryzacją i autentykacją użytkowników.
    - **UserModule**: Zarządzanie danymi użytkowników i ich uprawnieniami.
    - **ProductModule**: CRUD dla produktów.
    - **SyncModule**: Logika synchronizacji danych z platformami eCommerce.
    - **IntegrationModule**: Obsługa konfiguracji integracji z platformami eCommerce.

- **Frontend**:
  - **Technologie**: React.js
  - **Komponenty**:
    - **Login**: Formularz logowania.
    - **Register**: Formularz rejestracji.
    - **Dashboard**: Podsumowanie stanu synchronizacji.
    - **ProductList**: Lista produktów z opcjami zarządzania.
    - **Settings**: Ustawienia konta i integracji.
    - **Logs**: Historia operacji i błędów.

### 5.2 Komponenty Systemu

- **AuthModule**: Zajmuje się logowaniem, rejestracją i zarządzaniem sesjami użytkowników.
- **UserModule**: Przechowuje i zarządza informacjami o użytkownikach oraz ich uprawnieniami.
- **ProductModule**: Umożliwia tworzenie, aktualizowanie, usuwanie oraz przeglądanie produktów.
- **SyncModule**: Obsługuje proces synchronizacji produktów i klientów pomiędzy OmniSync a platformami eCommerce.
- **IntegrationModule**: Pozwala na dodawanie, usuwanie i konfigurowanie integracji z platformami eCommerce.

### 5.3 Wykorzystywane Technologie

- **Backend**: Node.js, Nest.js, MySQL
- **Frontend**: React.js, Redux
- **Inne**: Docker (konteneryzacja), GitHub Actions (CI/CD), Jest (testowanie jednostkowe)

## 6. Dokumentacja i Wsparcie

### 6.1 Dokumentacja API

- **Endpointy**:
  - **Auth**:
    - POST `/api/auth/login`: Logowanie użytkownika.
    - POST `/api/auth/register`: Rejestracja nowego użytkownika.
  - **Products**:
    - GET `/api/products`: Pobierz listę produktów.
    - POST `/api/products`: Dodaj nowy produkt.
    - PUT `/api/products/:id`: Zaktualizuj produkt.
    - DELETE `/api/products/:id`: Usuń produkt.
  - **Integrations**:
    - GET `/api/integrations`: Pobierz listę integracji.
    - POST `/api/integrations`: Dodaj nową integrację.
    - DELETE `/api/integrations/:id`: Usuń integrację.

## 7. Plan Rozwoju

### 7.1 Fazy Rozwoju Projektu

#### Faza 1 (0-14 miesięcy):

- Implementacja podstawowych funkcji backendu i frontendu.
- Integracja z WooCommerce i Shopify.
- Testowanie jednostkowe i integracyjne.

#### Faza 2 (2-4 miesiące):

- Udoskonalenie UI/UX na podstawie feedbacku użytkowników.
- Testy akceptacyjne i poprawki.

#### Faza 3 (4-6 miesięcy):

- Rozszerzenie o dodatkowe platformy (OpenCart, Amazon).
- Optymalizacja wydajności i skalowalności systemu.
- Przygotowanie do produkcyjnego wdrożenia.

### 7.2 Harmonogram

- **Miesiąc 1-3**: Wstępna faza projektowania i implementacji.
- **Miesiąc 4-6**: Implementacja kluczowych funkcji i integracji.
- **Miesiąc 7-9**: Testowanie jednostkowe, integracyjne i akceptacyjne.
- **Miesiąc 10-12**: Udoskonalenie UI/UX i zbieranie feedbacku.
- **Miesiąc 13-14**: Finalne testy i przygotowanie do wdrożenia.
- **Miesiąc 15-16**: Wdrożenie do produkcji i monitorowanie.
