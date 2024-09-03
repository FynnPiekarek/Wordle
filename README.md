# Wordle Spiel mit Blazor

## Projektübersicht

Dieses Projekt ist ein Wordle Spiel, das von Grund auf mit Blazor entwickelt wurde. Es handelt sich um ein sechsbuchstabiges Wortspiel, bei dem der Spieler ein geheimes Wort erraten muss. Im Gegensatz zu den meisten Wordle Spielen, die nur fünf Buchstaben verwenden, habe ich beschlossen, den Schwierigkeitsgrad zu erhöhen, indem ich komplexere Wörter mit sechs Buchstaben einführe. Das Projekt wurde ohne die Verwendung eines Tutorials entwickelt, um den Lernprozess und das Verständnis für die Programmierung mit Blazor zu vertiefen. Eine API wurde verwendet, um die englischen Wörter zu beziehen.

## Setup

Um das Projekt auszuführen, müssen die folgenden NuGet-Pakete installiert werden:

1. **Blazor Bootstrap**
2. **Newtonsoft.Json**

## Algorithmus-Überlegungen

 Die Hauptidee besteht darin, das eingegebene Wort mit dem geheimen Wort zu vergleichen und dabei folgende Überlegungen zu berücksichtigen:

- **Richtige Buchstaben am richtigen Platz (Grün)**: Wenn ein Buchstabe sowohl im eingegebenen als auch im geheimen Wort an derselben Stelle vorkommt, wird dieser als "right" markiert.
- **Richtige Buchstaben am falschen Platz (Gelb)**: Wenn ein Buchstabe im geheimen Wort vorkommt, aber an einer anderen Position, wird dieser als "wrong" markiert.
- **Falsche Buchstaben (Grau)**: Buchstaben, die im geheimen Wort nicht vorkommen, werden als "empty" markiert.

Um all diese Faktoren berücksichtigen zu können verwendete ich ein Dictionary in dem Algorythmus.

## Benutzeroberfläche (UI)

Die Gestaltung der Benutzeroberfläche spielt eine wichtige Rolle in diesem Projekt, so das es Benutzer freundlich ist.

Ein besonders wichtiger Teil der Benutzeroberfläche ist die virtuelle Tastatur. Sie ermöglicht es dem Spieler, seine Buchstaben direkt in das Spiel einzugeben und bietet ihm eine bessere Übersicht über den Spielstand. Die Übersichtlichkeit haben wir dadurch erreicht, dass die Tasten der Tastatur die entsprechende Farbe annehmen. Mit diesem Feature kann der Benutzer auf einen Blick sehen, welche Buchstaben er noch nicht verwendet hat.






