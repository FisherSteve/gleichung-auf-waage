# Gleichungen auf der Waage

Eine interaktive Anwendung für den Mathematikunterricht: Gleichungen als Waagen darstellen, Summanden bewegen und lineare Gleichungssysteme durch Gleichsetzen lösen.

**[Online ausprobieren](https://gleichung-auf-waage.netlify.app/)**

## Starten

1. Die Datei [index.html](index.html) herunterladen. Auf GitHub dafür die Datei öffnen und **Download raw file** wählen. Alternativ das Repository über **Code → Download ZIP** herunterladen und entpacken.
2. `index.html` in einem aktuellen Browser öffnen, zum Beispiel Firefox, Chrome oder Edge.

Die Anwendung läuft vollständig im Browser und funktioniert auch ohne Internetverbindung. Installation und Anmeldung sind nicht erforderlich. Eigene Eingaben bleiben nur während der geöffneten Sitzung erhalten.

## Eine Gleichung untersuchen

- Ein Beispiel auswählen oder unter **Eigene Eingabe** eine Gleichung eingeben und auf **Auf die Waage** klicken.
- Einen Baustein anklicken oder auf die andere Schale ziehen. Unter **Summanden bewegen** lässt sich zwischen Seitenwechsel mit Vorzeichenwechsel und freiem Verschieben wählen.
- Über **Umformen** auf der jeweiligen Waage Terme zusammenfassen oder beide Seiten durch eine Zahl teilen. Die Division wird zunächst veranschaulicht und anschließend bestätigt.
- Mit **Rückgängig** einen Schritt zurückgehen, mit **Ausgangslage** die Waagen zurücksetzen. **Tafelansicht** vergrößert die Darstellung für die Vorführung.

Die Neigung zeigt die Wirkung einer Veränderung. Negative Terme und Brüche werden dabei als algebraische Werte behandelt.

## Gleichungssysteme und Gleichsetzen

Im Reiter **Gleichsetzen** stehen zwei Ausgangswaagen und eine gemeinsame Vergleichswaage bereit. Links sind von null verschiedene Vielfache von `y` erlaubt, rechts Terme mit `x` und Zahlen.

Über den Übertragen-Knopf an einer Ausgangswaage oder unter der Vergleichswaage wird die ganze rechte Seite übernommen. Sie kann auch auf die zugehörige Schale der Vergleichswaage gezogen werden. Beide Ausgangswaagen bleiben dabei erhalten.

**Beispiel „Erst durch 2 und 3 teilen“:**

```text
(I)   2y = 4x + 2
(II)  3y = 3x + 9
```

1. Beide rechten Seiten direkt übertragen: Die Vergleichswaage gerät aus dem Gleichgewicht. Die Terme stehen für `2y` und `3y`; die linken Seiten stimmen noch nicht überein.
2. Auf Waage (I) über **Umformen** durch `2` teilen und bestätigen. Auf Waage (II) durch `3` teilen und bestätigen. Änderungen an einer Ausgangswaage setzen die Vergleichswaage zurück.
3. Jetzt stehen dort `y = 2x + 1` und `y = x + 3`. Beide rechten Seiten erneut übertragen: Die Vergleichswaage bleibt im Gleichgewicht.
4. Die entstandene Gleichung durch Bewegen und Zusammenfassen zu `x = 2` umformen. Mit **x einsetzen** ergibt sich `y = 5` und damit die Lösung `(2 | 5)`.

Entscheidend sind gleiche linke Seiten: Auch zweimal `2y` erlaubt das Gleichsetzen. Bei unterschiedlichen linken Seiten weist die Vergleichswaage auf die fehlende Voraussetzung hin und bietet keine LGS-Lösung aus diesem Vergleich an. Dieser Hinweis bleibt auch dann sichtbar, wenn die rechten Seiten bei einem einzelnen Zahlenwert zufällig gleich sind, etwa bei `y = 0`.

**Neu zeigen** leert nur die Vergleichswaage; die umgeformten Ausgangsgleichungen bleiben erhalten.

## Eigene Eingaben

Erlaubt sind `x`, `y`, Klammern, Dezimalzahlen mit Komma oder Punkt und Brüche. Multiplikation lässt sich zum Beispiel als `3x`, `3*x` oder `3(x + 1)` schreiben. Jeder Summand außerhalb einer Klammer erhält einen eigenen Baustein.

Beispiele für den LGS-Modus:

```text
y = 4x + 1       und   y = x + 7
2y = 4x + 2      und   3y = 3x + 9
-2y = x - 4     und   y = 2x + 1
```

Im LGS-Modus muss links ausschließlich ein Vielfaches von `y` stehen. Der Faktor darf auch negativ oder ein Bruch sein, aber nicht null. Rechts darf kein `y` vorkommen. Produkte zweier Variablen wie `xy` und Divisionen durch Variablen werden nicht unterstützt.
