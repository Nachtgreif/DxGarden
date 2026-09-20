# Changelog

Dieses Changelog dokumentiert umgesetzte Produktänderungen. Vorschläge und
Planungen stehen stattdessen in der [öffentlichen Roadmap](ROADMAP.md).

## Unreleased

Noch keine Änderungen vorgemerkt.

## 2.2.0 – 2026-09-20

- Einleitung und Kapitel erscheinen unmittelbar mit dem sichtbaren
  Lektionsknoten; ein geöffnetes Inhaltsfenster ist nicht mehr Voraussetzung.
  Beim Einklappen verschwinden Kapitel rückwärts und danach die Knoten mit der
  vereinbarten kurzen Verzögerung.
- Glossar- und Zusatzfenster skalierbar gemacht. Normale WordPress-Seiten
  erhalten dafür eine eigene Auswahl; das Einstellungsfenster bleibt fest.
- Lektionsfenster weiter oben platziert und zuverlässig vom unteren Linkmenü
  freigehalten.
- Schließen eines Medienfensters vom Inhalt des Hauptfensters entkoppelt, damit
  Kapitel und Scrollposition unverändert bleiben.
- Medien wahlweise als Textlink oder kleines 96 × 72 Pixel großes
  Vorschaubild verknüpft; das Originalmedium wird nicht dupliziert.
- Drei Kapitelbedienelemente im Lektionskopf dauerhaft gleichmäßig angeordnet
  und lange Titel auf den tatsächlich verfügbaren Raum begrenzt.
- Glossar-Mouseover gegen hängenbleibende und verspätete Hinweise abgesichert;
  Fokus, Touch, Scrollen, Escape und Inhaltswechsel teilen denselben
  Aufräumweg.
- Glossarbegriffe per Mehrfachaktion veröffentlichbar oder als Entwurf
  speicherbar.
- Doppelte native Garden-Themenauswahl aus Blockeditor und klassischem Editor
  entfernt; die verständliche DxGarden-Zuordnung bleibt die einzige Eingabe.
- Instrument Sans lokal einschließlich Lizenz ausgeliefert, in WordPress
  registriert und als einheitliche Theme- und Graphschrift verwendet.
- Das untere Linkmenü bewahrt zwei unmittelbar benachbarte Striche, wobei je
  ein `|` zum angrenzenden Link gehört.
- Vollständige Regression sowie frische Installation, Deaktivierung,
  Reaktivierung, Rückkehr auf 1.1.3 und erneutes Update auf 2.2.0 geprüft.

## 2.1.0 – 2026-09-19

- Blockierenden Fehler der WordPress-Elternauswahl behoben: Ein neues
  Garden-Thema lässt sich zuverlässig direkt an das virtuelle Zentrum hängen,
  wird intern mit Elternwert `0` gespeichert und erscheint sofort im ersten
  Ring. Die Auswahl zeigt den Graph-Titel mit `(Zentrum)` statt `Keine`.
- WordPress-natives Glossar ergänzt: Gutenberg-Inhalt, Autor, Revisionen,
  kurze Mouseover-Erklärung, ausführlicher Inhalt, Aliasse, verwandte Begriffe,
  Suche und Verknüpfung markierter Begriffe im Beitragseditor.
- Glossar wahlweise im Portalring, im unteren Linkmenü, an beiden Stellen oder
  in keinem Menü verfügbar. Das Portal verwendet ein festes Symbol eines
  aufgeschlagenen Buches.
- Desktop-, Tastatur- und Mobilbedienung für Glossarbegriffe umgesetzt:
  Kurzdefinition bei Hover/Fokus beziehungsweise erster Berührung,
  ausführlicher Inhalt im Garden-Fenster und normaler Link als Rückfallebene.
- Den WordPress-Zitatblock um den Stil `Merksatz` ergänzt. Akzentbalken und
  leicht hellere Fläche folgen den gewählten Theme-Farben; normale Zitate
  bleiben unverändert.
- Das untere Linkmenü erzeugt `||` ohne zusätzlichen Zwischenraum und ohne
  Strich bei nur einem Link. Veraltete Portaldaten führen nicht mehr
  unerwartet auf eine vollständige Browserseite.
- Manuelle WordPress-Aktualisierungsprüfungen leeren nun auch den eigenen
  Manifestcache; im normalen Betrieb bleibt der Sechs-Stunden-Cache erhalten.
- Deutsche Verwaltungsbegriffe mit korrekten Umlauten versehen und eine
  Warnung durch fremde Blockeditor-Kontexte beseitigt.
- Vollständige Regression, Migration, Paketinstallation, Rückkehr auf 1.1.3
  und erneutes Update auf 2.1.0 ohne Fehler geprüft.

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
