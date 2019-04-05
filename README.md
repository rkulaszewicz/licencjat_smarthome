# Streszczenie
  W projekcie „Inteligentny Dom” wykorzystaliśmy układy scalone ESP82661.Zostały one wmontowane w listwę zasilającą, a dzięki możliwości zaprogramowania ich w języku C oraz GPIO2, umożliwiają otwarcie lub zamknięcieprzepływu prądu. Układy poprzez moduł Wi–Fi łączą się z serwerem, do którego wysyłają informacje o aktualnym stanie urządzenia oraz odbierają sygnały zarządzające. Użytkownik może włączać lub wyłączać przepływ prądu korzystając z aplikacji mobilnej bądź strony internetowej. W obu przypadkach posłużyliśmy się językiem Python, lecz używając różnych bibliotek oraz frameworków: Twisted–Kivy na system Android, Flask dla strony internetowej.
  Program wymaga od użytkownika rejestracji oraz każdorazowego logowania. Aby odizolować się od niechcianego działania osób trzecich, autoryzacja odbywa się po stronie serwera, poprzez rozszerzenie Flask – SQLAlchemy3. Po zalogowaniu, przed pierwszym zastosowaniem urządzenia, należy zarejestrować układ ESP podając jego adres IP. Komunikację zaimplementowaliśmy przez urlib, z kolei kontakt z modemem 3G jest możliwy poprzez serial port.
# Inteligentny dom

Projekt stworzony podczas zajęć na Uniwersytecie Gdańskim, mający na celu stworzeniu oprogramowania pozwalającego kontrolować urządzenia w docelowym obiekcie. W repozytorium znajduje się nasza praca licencjacka. 

## Wykorzystano:
* [Flask](http://flask.pocoo.org/)
* [Kivy](https://kivy.org/#home)
* [Twisted](https://twistedmatrix.com/trac/)
* [SqlAlchemy](https://www.sqlalchemy.org/)

## Autorzy:
* Ewelina Mazur
* Rafał Kulaszewicz
* Maciej Marzec

## [LINK](https://github.com/dzyzus/inteligentny-dom) do repo z kodem projektu.
