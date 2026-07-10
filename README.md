# Alertă Sigură — prima versiune

Deschide `index.html` într-un browser. La prima intrare ca administrator, creezi tu parola ta personală. Nu există o parolă standard afișată în aplicație. Fluxul clientului are verificare cu cod; pentru previzualizare, codul de test este `123456`.

Aceasta este o demonstrație locală: datele, utilizatorii aprobați și alertele sunt salvate doar în browserul curent. Pentru aplicația reală sunt necesare un server securizat, Google Sign-In real, o bază de date și notificări către administrator.

Pentru coduri trimise automat pe e-mail, serverul va genera câte un cod unic, cu expirare, și îl va trimite dintr-o adresă de e-mail configurată de administrator. Codul de test nu este folosit în versiunea reală.

Funcția Action Button și comanda Siri cer o aplicație iPhone nativă (nu pot fi activate direct de o pagină web). Acest prototip stabilește interfața și fluxul de alertă.

## Distribuire și actualizări private

Nu este necesar Google Play acum. După ce aplicația reală este pregătită, administratorul publică versiuni noi pe serverul propriu:

- **PC:** utilizatorii deschid linkul privat; la următoarea deschidere primesc automat versiunea nouă.
- **Android:** se poate instala privat printr-un link APK controlat de administrator. Utilizatorii autorizați sunt singurii care pot intra, chiar dacă au fișierul aplicației.
- **iPhone:** aplicația poate fi testată privat prin TestFlight, cu adresele aprobate de administrator. Pentru distribuire permanentă în afara App Store, Apple impune metodele sale de distribuire și un cont Apple Developer.

Publicarea în Google Play sau App Store poate fi făcută mai târziu, numai când administratorul decide. O actualizare nu oferă automat acces: verificarea Gmail-ului aprobat rămâne activă pe server.
