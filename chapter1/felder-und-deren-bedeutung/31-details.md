# 2.1 Details

---

1. **Typ**
2. **Priorität**
3. **betrifft Version\(en\)**
4. **Stichwörter**
5. **Branch**
6. **Status**
7. **Lösung**
8. **Lösungsversion\(en\)**

## 1. Typ

Dieses Feld wird dazu genutzt die Aufgabe zu spezifizieren. Die Auswahlmöglichkeiten sind hier:

* **Aufgabe**
  * Ein standard Aufgabentyp, wie zum Beispiel eine Änderung des Frontend-Bereichs
* **Bug**
  * Ist z.B. ein schwerwiegender Fehler in der Funktionalität der Live-Seite aufgetreten, wird dieser Vorgangstyp gewählt. Dadurch wird signalisiert, dass dieses Ticket wichtig ist und so schnell wie möglich bearbeitet werden sollte.
* **Neue Funktion**
  * Ein neues Modul, bzw. eine neue Funktionalität soll in die Seite eingebaut werden
* **Verbesserung**
  * Ein bestehendes Modul, bzw. eine bestehende Funktionalität soll erneuert oder optimiert werden
* **Epic**
  * Dies ist eine "Container" für Tickets. Darin werden kleine Tickets aufgelistet die unter der Aufgabe laufen.
* **Story**

## 2. Priorität

Durch dieses Feld wird ein Ticket priorisiert. Die Auswahlmöglichkeiten sind hier:

* **Normal**
  * Dies ist der Standardwert für dieses Feld. Das Ticket wird normal \(nach Erstellungsreihenfolge\) auf dem Board angezeigt.
* **Blocker**
  * Dieser Wert blockt jegliche Aufgaben, solange dieses Ticket nicht erledigt wurde. In Notfällen zu verwenden \(wie z.B. Server down\)
* **Hoch **
  * Ein Ticket mit der Priorität hoch wird als erstes auf dem Board angezeigt \(Erstellungsreihenfolge wird ignoriert\).
* **Unwesentlich**
  * Unwesentliche Tickets werden als letztes auf dem Board angezeigt \(Erstellungsreihenfolge wird ignoriert\).

## 3. betrifft Version\(en\)

Dieses Feld gibt an, welche Version des Entwicklungsvorganges von der Aufgabe betroffen ist. Z.B. Browerdarstellung muss in Version 1.6 gefixt werden.  
**Dieses Feld wird meist nicht mit angegeben \(findet nur in seltenen Fällen Verwendung\).**

## 4. Stichwörter

In diesem Feld werden Wörter angegeben \(z.B. Theming, Sitebuilding, Firma xyz\) die die Tickets kategorisieren sollen. Wird auf eines dieser Stichwörter geklickt, so werden alle Tickets aufgelistet, die diesem Stichwort zugeordnet sind, bzw. dasselbe Stichwort tragen.

## 5. Branch

In diesem Feld wird eingetragen unter welchem Git-Branch die Aufgabe gelöst wurde \(z.B. feature/DSAG-1971\).

## 6. Status

Dieses Feld wird automatisch ausgefüllt, wenn ein Ticket auf dem Board verschoben wird, bzw. bei dessen Erstellung. Hier wird angezeigt in welcher Phase sich das Ticket gerade befindet. Mögliche Status sind:

* **Planung**
  * Tickets mit diesem Status werden momentan geplant \(Projektmanagement\) und sind nicht sichtbar auf dem Board, d.h. sie sind nicht zur Bearbeitung freigegeben.
* **Offen**
  * Tickets mit diesem Status wurden vom Projektmanagement vom Kunden aufgenommen, aber noch nicht bearbeitet. Diese Tickets sind nicht zur Bearbeitung freigegeben.
* **Aufgaben \(ToDo\)**
  * Tickets mit diesem Status werden in der ersten Spalte auf dem Board ausgegeben und zeigen an, dass sie nun earbeitet werden können.
* **In Arbeit**
  * Dieser Status gibt an, dass ein Mitarbeiter dieses Ticket gerade bearbeitet.
* **Testing \(CI\)**
  * Nach einem erfolgreichen Commit \(Code-Veränderung die im Gitlab veröfentlicht wurde\) läuft ein automatisierter Test durch, dass diese Veränderung die Webseite nicht zerstört \(Funktionialität wird gewährleistet\). Das Ticket liegt solange unter diesem Status auf dem Board, bis die automatisierten Tests durchgelaufen sind. Danach erfolg der Code Review.
* **Code Review**
  * Tickets mit diesem Status werden von Mitarbeitern, die das Ticket nicht bearbeitet haben, kontrolliert \(Mehr-Augen-Prinzip\). Hier wird der Code auf eventuelle logische Fehler, die bei den automatisierten Tests nicht aufgefallen sind, überprüft und verifiziert.
* **Review**
  * Tickets mit diesem Status werden vom angegenen Mitarbeiter auf ihre Funktion geprüft. Wird zum Beispiel ein Export verändert, überprüft ein unabhängiger Mitarbeiter die gewünschte, geänderte Funktion auf die korrekte Ausführung. 
* **Deploy to Stage**
  * Tickets mit diesem Status wurden getestet und freigegeben für die stage. 
* **to Stage**
  * Tickets mit diesem Status werden momentan auf die stage verschoben.
* **Stage**
  * Tickets mit diesem Status wurden zur stage deployed und werden nun vom Kunden abermals auf ihre Funktionalität überprüft.
* **to Live \(Deploy\)**
  * Tickets mit diesem Status wurden vom Kunden verifiziert und sollen auf die live Webseite gebracht werden.
* **Done**
  * Tickets mit diesem Status wurden erfolgreich in die Live-Webseit integriert und werden momentan dokumentiert.
* **Fertig**
  * Tickets mit diesem Status sind fertig und landen im Archiv.

## 7. Lösung

**Dieses Feld wird benutzt**

## 8. Lösungsversion\(en\)

Dieses Feld wird ausgefüllt nachdem das Ticket deployed wurde. Hier wird angegeben in welcher Version das Problem gelöst wurde \(z.B. 1.6\).

