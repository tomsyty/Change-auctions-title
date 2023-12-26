## Szybka zmiana tytułu aukcji
To rozszerzenie pozwala na łatwą i szybką zmianę tytułu aukcji bezpośrednio na liście ofert bez konieczności przechodzenia przez cały proces edycji oferty.

Jest to rozszerzenie do przeglądarki Chrome. Wszystkie rozszerzenia testuję tylko dla systemu Windows 10 i najnowszej wersji przeglądarki.

**Instrukcja instalacji:**
1. Pobierz rozszerzenie "change_auctions_title.zip" z listy plików widocznej powyżej i rozpakuj je tam gdzie zamierzasz je trzymać.
2. Kliknij ikonę menu rozszerzeń w prawym górnym rogu okna przeglądarki (ikona puzzla)
![chrome_extensions_menu_icon](https://github.com/tomsyty/Change-auctions-title/assets/41838854/55ba680b-46d4-465e-b85d-0624293c840c)
lub z menu przeglądarki wybierz "Rozszerzenia - Zarządzaj rozszerzeniami".
3. Włącz "Tryb dewelopera" w prawym górnym rogu okna przeglądarki
![chrome_enabled_developer_mode](https://github.com/tomsyty/Change-auctions-title/assets/41838854/9cf71d79-e775-4541-9164-dce74a8f2fde)
4. Kliknij przycisk "Załaduj rozpakowane"<br/>
![chrome_extensions_load_unpacked_button](https://github.com/tomsyty/Change-auctions-title/assets/41838854/f6f2b331-1841-43a5-b0ee-6297f10f035c)
5. Wybierz folder z uprzednio pobranym i rozpakowanym rozszerzeniem.
6. Po załadowaniu rozszerzenia otworzy się strona jego opcji, gdzie wymagane będzie uzupełnienie danych Client ID i Client Secret. Uzyskasz je rejestrując aplikację na stronie [developer.allegro.pl](https://developer.allegro.pl/)<br/>
    <details>
    <summary>Instrukcja rejestracji aplikacji</summary>
    
    1. Upewnij się że zalogowany jesteś na konto Allegro w ramach którego działać będzie aplikacja. Jeśli nie, wyloguj się (klikając ikonę obok nazwy użytkownika i wybierając "Wyloguj") a następnie zaloguj na właściwe konto.
    
    2. Kliknij "Zarządzaj API" - "Moje aplikacje".
    3. Kliknij przycisk "Zarejestruj aplikację".  
    4. W formularzu rejestracji aplikacji Allegro podaj następujące dane:
        - **Nazwa aplikacji:** dowolna, np. "Change Auctions Title"
        - **Wybierz rodzaj aplikacji:** zaznacz pierwszą opcję ("Aplikacja ma dostęp do przeglądarki, w której użytkownik loguje się do Allegro (np. aplikacja na serwerze albo plik wykonywalny)").      
          ![allegro_application_type_code_flow](https://github.com/tomsyty/Change-auctions-title/assets/41838854/f7e24de4-1ac1-4a02-b066-24ea3027198f)
        - **Ścieżka aplikacji:** na stronie opcji rozszerzenia zaznacz i skopiuj tekst widniejący przy parametrze **Ścieżka aplikacji**. Jest to unikalny adres aplikacji w domenie chromiumapp.org pod który Allegro będzie przesyłać kod autoryzujący i tokeny dostępowe.
        - **Uprawnienia aplikacji:** zaznacz następujące uprawnienia: `allegro:api:sale:offers:read` `allegro:api:sale:offers:write` (sekcja **Zarządzanie ofertami**), `allegro:api:profile:read` (sekcja **Dane osobowe**).
        - Zaznacz `* Znam i akceptuję regulamin REST API Allegro`.
        - Kliknij przycisk "Zarejestruj".
    5. Aplikacja zostanie zarejestrowana. Kliknij "Szczegóły" aby odczytać Client ID i Client Secret. Zaznacz i skopiuj parametr Client ID, wklej go na stronie ustawień rozszerzenia w polu Client ID. Kliknij "Pokaż" przy parametrze Client Secret, aby odsłonić domyślnie zamaskowaną wartość tego parametru, zaznacz i skopiuj parametr Client Secret, wklej go na stronie ustawień rozszerzenia w polu Client Secret. Zamknij okno ze szczegółami aplikacji.
    6. Kliknij "Zapisz" a następnie "Zaloguj" na stronie opcji rozszerzenia. Zostaniesz przeniesiony na stronę Allegro gdzie musisz potwierdzić że kontynuujesz jako zalogowany użytkownik:

        ![allegro_confirm_account_dialog](https://github.com/tomsyty/Change-auctions-title/assets/41838854/7485140b-6dd8-4e74-aea6-823a9746b141)<br/>
    7. Kliknij przycisk "Kontynuuj".
    8. Zostaniesz przeniesiony na stronę Allegro z pytaniem czy chcesz powiązać swoje konto z aplikacją:<br/>
      ![allegro_account_linking_question_allegro-api-sale-offers-read, allegro-api-sale-offers-write, allegro-api-profile-read](https://github.com/tomsyty/Change-auctions-title/assets/41838854/4aa89ef8-32b2-44b3-b27e-57d3d84ef80b)<br/>
    9. Kliknij przycisk "Tak, powiąż konto".
    10. Na stronie opcji rozszerzenia pojawi się komunikat o zalogowaniu wraz z nazwą użytkownika.
    </details>
7. Jeżeli miałeś otwartą stronę "Mój asortyment", odśwież ją, celem załadowania rozszerzenia.
8. Najedź kursorem myszy na tytuł aukcji który chcesz zmienić i wciśnij <kbd>Ctrl</kbd> + <kbd>Insert</kbd> (jest to domyślny skrót klawiaturowy, możesz go zmienić na stronie opcji rozszerzenia). Tytuł aukcji podświetli się na zielono i możliwa będzie jego edycja.
   ![sample_auction_change_edit_mode](https://github.com/tomsyty/Change-auctions-title/assets/41838854/b11618be-888a-4064-97b9-a39df2e5f07b)
