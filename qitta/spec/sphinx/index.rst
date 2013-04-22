.. Movie Database with Apex documentation master file, created by
   sphinx-quickstart on Mon Apr 22 16:06:30 2013.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


Beschreibung und Datenbankschema
================================

Im Rahmen der Studienarbeit Entwicklung von Webanwendungen soll eine Apex
Applikation realisiert werden. Das gewählte Thema umfasst eine Film Metadaten
Plattform, ähnlich dem großem IMDb Vorbild. (www.imdb.com) 

Die Film-Datenbank soll die grundlegende Metadaten verwalten können und folgende
Funktionalität bieten:

 * Film Metadaten inklusive Poster-Art + Fan-Art
 * Film Informationen auswertbar nach Genre bzw benutzerdefinierten Tags
 * Informationen zum Regisseur/Drehbuchautor
 * Informationen zu Schauspielern inkl. Foto + Statistiken
 * Verschiedene statistische Auswertungsmöglichkeiten von
   Film/Genre/Personen-Metadaten
 * Rating System
 * Erstellen von Favoriten-Listen
 

Im folgenden ist das Normalisiertes Datenbankschema für die o. g. Applikation:

.. image:: ./dataschema.png


Main View
---------

.. image:: ./mainview.png
  
**Inhalt**:

 * Hauptseite mit Suchfunktion
 * Kürzlich hinzugefügte Filme anzeigen
 * Links zur **Movies**, **Genre**, **Persons** und **Statistics** Seite

Movie View
----------

.. image:: ./movieview.png

**Inhalt**:

 * Anzeige von Film-Metadaten, Poster-Art, Fan-Art, Crew und Cast Informationen im
   oberen Bereich
 * Anzeige von ,,Similar Movies'' im unteren Bereich
 * Cast/Crew und Similar Movies leiten auf die jeweilige spezialisierte Seite
   weiter

Person View
-----------

.. image:: ./actorview.png

* Anzeigen von Schauspieler-Photo und Biografie im oberen Bereich
* Anzeigen von Filmen in denen der Schauspieler mitspielt im unteren Bereich


Statistics
----------

.. image:: ./statistics.png

**Inhalt**:

Anzeige von verschiedenen Statistiken wie z.B.:

 * Liste der besten/schlechtesten Filme
 * Statistische Auswertung nach Laufzeit, Herstellungsland, Rating, etc.
 * Genre Charts (z.B. Tortendiagramm)
 * Person Charts nach Filmgenre
 * Rating Chart
 * Statistiken zu gesehenen und eingetragenen Filmen
 * Favoriten Listen und Statistiken erstellen  
