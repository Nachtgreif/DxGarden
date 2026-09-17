# Changelog

Dieses Changelog dokumentiert umgesetzte Produktänderungen. Vorschläge und
Planungen stehen stattdessen in der [öffentlichen Roadmap](ROADMAP.md).

## Unreleased

Noch keine Änderungen vorgemerkt.

## 2.0.0 – 2026-09-18

- Lektionen in die normalen WordPress-Beiträge integriert; vorhandene
  Beitragseditoren, Medien, Revisionen, Status und direkte Artikel-URLs werden
  dadurch ohne parallele DxGarden-Inhaltsverwaltung genutzt.
- Unterthemen als hierarchische WordPress-Taxonomie umgesetzt. Vier
  Themenebenen und höchstens fünf gemischte Kinder aus Themen und Lektionen pro
  Elternpunkt werden zuverlässig geprüft.
- Portale und das Linkmenü unten rechts in normale WordPress-Seiten verlagert.
  Eine Seite kann unabhängig voneinander Portal, Linkmenüpunkt oder beides sein.
- Sichere, wiederholbare Migration der bisherigen Garden-Elemente,
  Portaleinstellungen, Redakteursbereiche und Tickets eingebaut. Vor der
  Umwandlung entsteht eine vollständige technische Sicherung.
- Autoren- und Redaktionsablauf in die vertrauten WordPress-Bereiche Beiträge,
  Seiten, Benutzer, Design und Website-Zustand eingeordnet. Arbeitskopien
  schützen veröffentlichte Texte fremder Autoren bis zu deren Zustimmung.
- Kapitel automatisch aus H2-Überschriften erzeugt; Einleitung vor der ersten
  H2 bleibt optional, H3 und kleinere Überschriften bleiben reiner Inhalt.
- Medien-Ergänzungen als WordPress-Detailsblock mit stabilen Ankern und
  Verknüpfung aus ausgewähltem Text oder kleinen Vorschaubildern umgesetzt.
- Einstellungsfenster oben rechts angeordnet. Bedienmodus, Bewegung sowie der
  neue Umschalter Farbraum/Individuell folgen der vereinbarten Darstellung.
- Im Farbraum-Modus wird das vollständige Schema aus „Akzent und Ringe“
  abgeleitet; im individuellen Modus bleiben alle Farben getrennt einstellbar.
  Dieselbe Auswahl steht für die Administrationsstandards bereit.
- Administrativen Reset ergänzt. Er setzt nur Darstellung, Physik und
  Farbmodus auf den Installationsstandard zurück; Inhalte, Benutzer,
  Zuordnungen und Besuchereinstellungen bleiben unberührt.
- Öffentliche Oberfläche auf Desktop und Mobil geprüft und das untere
  `||`-Menü auf kleinen Bildschirmen stabilisiert.
- Installations-, Deaktivierungs-, Reaktivierungs-, Migrations- und
  WordPress-Updateweg von 1.1.3 auf 2.0.0 automatisiert geprüft.

## 1.1.3 – 2026-09-17

- Offiziellen Veröffentlichungs- und Updatekanal in das Produkt-Repository
  `Nachtgreif/DxGarden` verlegt.
- WordPress-Updateprüfung auf das neue Manifest umgestellt und geprüft.
- Historische Versionen ohne veraltete Installationspakete dokumentiert.

## 1.1.2 – 2026-09-16

- WordPress-Updater korrigiert und seine Metadaten vervollständigt.
- Theme-Updateprüfung zusätzlich durch DxGarden Core abgesichert.

## 1.1.1 – 2026-09-16

- Öffentliche Bedienoberfläche an den freigegebenen Prototyp angeglichen.
- Desktop-/Mobil-Umschaltung und optionale Bedienhilfen in die Einstellungen
  zurückgeführt.
- Tastaturfokus auf tatsächliche Tastaturbedienung begrenzt.

## 1.1.0 – 2026-09-16

- Erste öffentliche installierbare Fassung von DxGarden Core und DxGarden
  Theme.
- Gemeinsame Versionierung, Updatekanal und SHA-256-Prüfung eingeführt.
