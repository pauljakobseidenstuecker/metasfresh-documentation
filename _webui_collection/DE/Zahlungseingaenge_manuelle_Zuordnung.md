---
title: Wie ordne ich eine einzelne Zahlung mehreren Rechnungen zu?
layout: default
tags:
  - Buchhaltung
  - Forderungen und Verbindlichkeiten
  - Zahlungseingänge (Forderungen)
lang: de
sequence: 20
ref: incoming_payments_manual_allocation
---

## Überblick
Wenn ein Kunde eine einzelne Zahlung leistet, um mehrere Rechnungen auf einmal zu begleichen, muss der erhaltene Betrag den jeweiligen Rechnungen *manuell zugeordnet* werden. Gehe hierzu wie folgt vor:

## Voraussetzungen
- Stelle sicher, dass Dir mehrere offene [Rechnungen](Zu_Auftrag_Rechnung_erstellen) vorliegen.

## Schritte
1. [Gehe ins Menü](Menu) und öffne das Fenster "Zahlungen".
1. [Erstelle einen neuen Zahlungseintrag](Neuer_Datensatz_Fenster_Webui).
1. Gib in das Feld **Geschäftspartner** einen Teil des Namens oder der Nummer des [Geschäftspartners](Neuer_Geschaeftspartner) ein und klicke auf den passenden Treffer in der <a href="Keyboard_Shortcuts_Liste#dropdown" title="Dynamisches Suchfeld (Autocomplete)">Dropdown-Liste</a>.
1. Wähle die **Belegart** *Zahlungseingang* aus.
1. Wähle die zur Rechnung passende **Währung** aus.
1. Gehe zur Registerkarte "Manuelle Zuordnung" unten auf der Seite und klicke auf !["Neu hinzufügen"](assets/Neu_hinzufuegen_Button.png). Es öffnet sich ein Overlay-Fenster.
1. Trage die **Rechnung** ein, für die Du die Zahlung erhalten hast.
 >**Hinweis 1:** Drücke die [`LEERTASTE`](Keyboard_Shortcuts_Liste), um eine Auswahl verfügbarer, offener Rechnungen des Geschäftspartners zu sehen.<br><br>
 >**Hinweis 2:** Der **Betrag** wird automatisch aus der Rechnung übernommen.

1. Klicke auf "Bestätigen", um das Overlay-Fenster zu schließen und die Rechnung zur Liste hinzuzufügen.
 >**Hinweis:** Wiederhole die Schritte 6 bis 8 für alle Rechnungen, die mit der erhaltenen Zahlung beglichen wurden.

1. [Stelle den Beleg fertig](BelegverarbeitungFertigstellen).
1. Um den Status der einzelnen Rechnungen zu überprüfen, gehe zur Registerkarte "Zuordnungen" und [zoome](Zoomen_in_Tabellenfeld) in das Feld in der Spalte **Rechnung** der jeweiligen Zuordnungszeile.

| **Hinweis:** |
| :--- |
| Die manuellen Zahlungszuordnungen der Rechnung kannst Du ebenfalls unter dem Menüpunkt "[Manuelle Zahlung Zuordnungen](Menu)" übersichtlich einsehen. |

## Beispiel
<kbd><img src="assets/Zahlungseingaenge_manuelle_Zuordnung.gif" alt="GIF: Zahlungseingänge manuelle Zuordnung"></kbd>
