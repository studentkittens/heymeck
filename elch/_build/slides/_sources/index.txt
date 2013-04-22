.. apex documentation master file, created by
   sphinx-quickstart on Mon Apr 22 15:51:06 2013.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


Musicbrowser
============

Christopher Pahl (MN 01271710)

Datenbankschema
---------------

.. image:: ./normalized.png
   :width: 700

Beschreibung
------------

Der Musicbrowser soll eine Übersicht über die eigene Musiksammlung bieten. 
Er bietet dazu eine Liste von Songs bei dem jedes Feld mit einer Detailview verlinkt ist.
So soll nach einem Klick auf einem Künstlernamen Details zu diesem angezeigt werden. 

Zudem soll eine zusätzliche Seite mit Statistiken über die Datenbank
implementiert sein. 

Da man oft mehr als eine Playlist hat, soll diese mittels eines Dropbdows
ausgewählt werden können.

Playlist
--------

    .. image:: ./queue.png
       :width: 400

    - Auswahl der aktuellen Playlist in einem Dropdown.
    - Anzeige einer Playlist als Liste von Songs mit Artist/Album/Title.
    - Verlinkung auf Statistics View.

Artist View
-----------
    
    **Beispielbild:**

        .. image:: ./artist.png
           :width: 120

    **Inhalt:**

        - Anzeige eines Künstlerbildes und der Similar Artists.
        - Anzeige einer Liste von Alben des Künstlers, die jeweils auf die 
          entsprechenden Albumview verlinken. Dazu ein Cover-Thumbnail.

Album View
----------

    **Beispielbild:**

        .. image:: ./album.png

    **Inhalt:**

        - Anzeige des Albumcovers.
        - Anzeige der Lieder innerhalb des Albums, die jeweils auf die entsprechenden Titleviews verlinken.

Title View
----------
    
    **Beispielbild:**

        .. image:: ./title.png

    **Inhalt:**

        - Anzeige des Liedtitels, Genre und Dauer.
        - Anzeige eines Liedtextes.

Statistics
----------

    **Inhalt:**

        - Anzeige verschiedener Diagramme:

            * Genre Pie-Chart (Aufteilung der Genres)
            * Duration Bar Chart (Längste/Kürzeste Lieder)
            * Künstlerverteilung (wieviel Songs von welchen Künstler)
            * ... 

