# Specyfikacja Projektu OmniSync (Wersja MVP)

## Nazwa Projektu
**OmniSync** - Synchronizacja danych produktów eCommerce

## Cel Projektu
OmniSync to uniwersalna platforma umożliwiająca dwukierunkową synchronizację produktów między różnymi sklepami internetowymi a centralnym systemem zarządzania. Wersja MVP wspiera integrację z WooCommerce i Shopify.

## Zakres Projektu
- Integracja z WooCommerce i Shopify
- Dwukierunkowa synchronizacja produktów
- Bezpieczne przechowywanie i przesyłanie danych
- Interfejs użytkownika do zarządzania integracjami
- Interfejs użytkownika do zarządzania integracjami, zoptymalizowany pod kątem przeglądarek Google Chrome, Safari, Firefox

## 1. Wymagania Funkcjonalne
- **Rejestracja i logowanie**: Użytkownicy mogą zakładać konta i logować się do systemu.
- **Zarządzanie integracjami**: Użytkownicy mogą dodawać i konfigurować integracje z WooCommerce i Shopify.
- **Synchronizacja produktów**: System automatycznie synchronizuje dane produktów między sklepami a OmniSync.
- **Panel administracyjny**: Umożliwia zarządzanie produktami, przeglądanie logów synchronizacji i konfigurację ustawień.

## 2. Wymagania Niefunkcjonalne
- **Bezpieczeństwo**: Dane przesyłane między systemami są szyfrowane przy użyciu klucza SSH wygenerowanego na urządzeniu użytkownika.
- **Wydajność**: System musi zapewniać szybką i niezawodną synchronizację danych.
- **Skalowalność**: Architektura systemu powinna umożliwiać łatwe dodawanie nowych funkcjonalności i integracji.

## 3. Architektura Systemu
### Backend (Node.js + Nest.js)
OmniSync składa się z kilku modułów:
- **AuthModule**: zarządzanie autoryzacją użytkowników
- **UserModule**: zarządzanie użytkownikami i ich konfiguracjami
- **ProductModule**: CRUD dla produktów
- **SyncModule**: logika synchronizacji danych z WooCommerce i Shopify
- **IntegrationModule**: obsługa konfiguracji integracji z platformami eCommerce

### Frontend (React.js)
Aplikacja frontendowa zawiera komponenty takie jak:
- **Login**: formularz logowania
- **Register**: formularz rejestracji
- **Dashboard**: podsumowanie stanu synchronizacji
- **ProductList**: lista produktów z opcjami zarządzania
- **Settings**: ustawienia konta i integracji
- **Logs**: historia operacji i błędów

Struktura aplikacji obejmuje strony (Home, Dashboard, Products, Settings, Logs), serwisy (AuthService, ProductService, SyncService) oraz komponenty (formularze, tabele, przyciski).

## 4. Integracje z Platformami eCommerce
- **WooCommerce**: Integracja z WooCommerce wykorzystuje OAuth1 do autoryzacji i umożliwia operacje takie jak pobieranie, dodawanie, aktualizowanie i usuwanie produktów.
- **Shopify**: Integracja z Shopify wykorzystuje OAuth2 do autoryzacji i obsługuje operacje pobierania, dodawania, aktualizowania i usuwania produktów.

## 5. Plan Rozwoju i Harmonogram
### Faza 1 (0-2 miesiące)
- Implementacja podstawowych funkcji backendu i frontendu
- Integracja z WooCommerce i Shopify
- Testowanie jednostkowe i integracyjne

### Faza 2 (2-4 miesiące)
- Dodanie zaawansowanych funkcji (szczegółowe logowanie operacji)
- Udoskonalenie UI/UX na podstawie feedbacku użytkowników
- Testy akceptacyjne i poprawki

### Faza 3 (4-6 miesięcy)
- Rozszerzenie o dodatkowe platformy (OpenCart, Amazon)
- Optymalizacja wydajności i skalowalności systemu
- Przygotowanie do produkcyjnego wdrożenia

## 6. Testowanie
- **Testy jednostkowe**: Testowanie pojedynczych funkcji.
- **Testy integracyjne**: Testowanie współpracy między komponentami.
- **Testy akceptacyjne**: Weryfikacja zgodności z wymaganiami użytkowników.

## 7. Wdrożenie
- **CI/CD**: Automatyzacja wdrażania (GitHub Actions).
- **Monitoring**: Prometheus i Grafana do monitorowania systemu.

## 8. Dokumentacja i Wsparcie
- **Dokumentacja API**: Szczegółowa dokumentacja endpointów.
- **Instrukcje użytkownika**: Przewodniki konfiguracji i użycia.
- **Wsparcie techniczne**: System zgłaszania błędów i propozycji usprawnień.

## Podsumowanie
Projekt OmniSync zapewni kompleksowe rozwiązanie do synchronizacji produktów między sklepami internetowymi, zaczynając od WooCommerce i Shopify. Skupienie się na bezpieczeństwie, wydajności i skalowalności gwarantuje solidne fundamenty dla dalszego rozwoju i rozszerzenia funkcjonalności.
