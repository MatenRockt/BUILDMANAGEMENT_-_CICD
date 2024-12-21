Dies ist ein einfaches Taschenrechner-Projekt, implementiert mit Gradle-Tasks. Die Anwendung ermöglicht es Benutzern, grundlegende mathematische Operationen wie Addition, Subtraktion, Multiplikation und Division durchzuführen. Es gibt eine klare Task-Struktur, bei der einige Tasks von anderen abhängen.

Projektaufbau

Das Projekt besteht aus mehreren Gradle-Tasks:

Task: taskA

Gibt eine Begrüßungsnachricht und eine Abschlussnachricht aus.

Wird von taskB ausgeführt.

Task: taskB

Hängt von taskA ab.

Gibt eine Nachricht aus, dass taskB ausgeführt wird und dass es von taskA abhängt.

Task: taschenrechner

Hängt von taskB ab.

Führt die Hauptlogik des Taschenrechners aus.

Zeigt ein Menü mit den Optionen Addition, Subtraktion, Multiplikation und Division an.

Führt die entsprechende Berechnung basierend auf der Benutzerauswahl aus.

Verwendet eine Hilfsmethode berechne zur Durchführung der Operationen.

Task: taskC

Hängt von taschenrechner ab.

Gibt eine Nachricht aus, dass der Taschenrechner abgeschlossen ist und taskC ausgeführt wird.

Features

Interaktives Menü:

Benutzer können eine Option für die gewünschte mathematische Operation auswählen.

Validierung:

Überprüft Benutzereingaben auf ungültige Werte (z. B. Division durch Null oder ungültige Zahlen).

Modularer Aufbau:

Jede Operation (Addition, Subtraktion, Multiplikation, Division) wird als separate Funktion behandelt.

Abhängigkeiten:

Die Gradle-Tasks sind so strukturiert, dass sie in der richtigen Reihenfolge ausgeführt werden.

Voraussetzungen

Java Development Kit (JDK) 8 oder höher

Gradle (Version 6.0 oder höher empfohlen)

Ausführung

Klone das Repository:

git clone https://github.com/dein-benutzername/taschenrechner.git
cd taschenrechner

Führe die Gradle-Tasks aus:

Task A:

gradle taskA

Task B:

gradle taskB

Taschenrechner:

gradle taschenrechner

Task C:

gradle taskC

Beispiel

Beispielausgabe

Taschenrechner-Auswahl:

Bitte waehlen Sie eine der folgenden Optionen:
1. Addiere zwei Zahlen
2. Subtrahiere zwei Zahlen
3. Multipliziere zwei Zahlen
4. Dividiere zwei Zahlen
Bitte eine Auswahl treffen (1-4): 1
Bitte geben Sie die erste Zahl ein:
5
Bitte geben Sie die zweite Zahl ein:
3
Das Ergebnis der addition ist: 8
