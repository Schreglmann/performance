# Hausübung

Dies ist eine einfache Web-App, die die Top-Stories von[Hacker News](https://news.ycombinator.com/news) über[ihre API](http://blog.ycombinator.com/hacker-news-api) anzeigt.

Leider hat es eine Reihe von Performance-Problemen, wie z.B.:

* Layout Thrashing
* Expensive Paints
* Unnötige Layouts
* Langlebiges und badly-timed JavaScript
* Schlechtes Touch Handling

Das Ziel ist es, die Probleme in der Applikation mit den DevTools zu finden

## Vorgehensweise
  * Beginne im Rendering Tab: Paint Flashing -> was wird repainted?
  * Scrolling Performance: welche Elemente beinflussen die Scrolling performance? Warum?
  * Gehe in den Performance Tab
    * Aufnahme vom Scrolling
    * Aufnahme von wenn man auf Details klickt
    * bei welchen Interaktionen verringern sich die FPS? Warum? 
    * Welche JS Funktionen beinflussen die Performance des Scrolling und der Anzeige der Details?
  * Gehe in den Layers Tab: werden unnötig viele Layers erstellt? Wenn ja aufgrund welches Code Snippets?

## Hinweise

* onScroll Funktion: Sind alle Funktionsaufrufe notwendig?
* slideIn der Details der Storys: gibt es einen einfacheren Weg diesen Effekt zu erzielen?
* CSS: Sind alle Styles notwendig? Gibt es duplizierte Styles?

## Abgabe

* eine Liste an Performanceproblemen, die ihr in der Applikation mit den Devtools gefunden habt
* Empfehlungen wie die Performance verbessert werden könnte
* Erklärung anhand der Pixel Pipeline: wo sind die Performance Bottlenecks? 
  * Javascript
  * Recalculate Style
  * Layout
  * Paint
  * Composite
* als Markdown oder PDF im Wiki oder eigenes Repo

