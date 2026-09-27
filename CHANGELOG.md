# Changelog

Dieses Changelog dokumentiert umgesetzte Produktänderungen. Vorschläge und
Planungen stehen stattdessen in der [öffentlichen Roadmap](ROADMAP.md).

## Unreleased

Noch keine Änderungen vorgemerkt.

## 2.3.0 – 2026-09-28

DxGarden 2.3.0 erweitert die bisherige WordPress-nahe Medienverwaltung um
wiederverwendbare Zusatzinhalte. Außerdem vervollständigt die Version die
bereits auf der geschützten PTU abgestimmten Farb- und Navigationskorrekturen.
Plugin und Theme tragen dieselbe Version.

## Änderungen

- **WordPress-native Zusatzinhalte:** Unter `Medien → Zusatzinhalte` können
  Autoren eigenständige Inhalte mit dem normalen Blockeditor erstellen. Ein
  Zusatzinhalt kann Texte, Tabellen, Bilder, Videos und weitere
  WordPress-Blöcke miteinander verbinden und besitzt Revisionen, Autor,
  Veröffentlichungsstatus sowie ein geeignetes Fensterprofil.
- **Einfache Einbindung in Beiträge:** Der Block `DxGarden-Zusatzinhalt`
  verbindet einen Beitrag mit einem vorhandenen Zusatzinhalt. Als Auslöser
  steht ein Textlink oder ein kleines Thumbnail zur Wahl. Entwürfe bleiben im
  öffentlichen Garden verborgen.
- **Vorschau aus dem tatsächlichen Inhalt:** Thumbnails werden standardmäßig
  automatisch aus dem Zusatzinhalt erzeugt. Ein eigenes Beitragsbild bleibt
  als freiwillige Alternative erhalten. Die Vorschau wird erst bei Bedarf
  geladen und übernimmt die eingestellten Theme-Farben.
- **Kontrollierte Vorschaugrößen:** Der Administrator legt Standard- und
  Maximalbreite fest. Autoren können die Breite innerhalb dieser Grenze am
  einzelnen Block wählen. Die Vorschau bleibt bewusst klein und verwendet ein
  festes Seitenverhältnis.
- **Geeignete Zusatzfenster:** Für kurze Erklärungen, gemischte Inhalte, breite
  Tabellen und hohe Inhalte stehen passende Startgrößen zur Verfügung. Die
  Fenster bleiben innerhalb sicherer Bildschirmgrenzen und lassen sich dort
  weiter anpassen.
- **Lesbare echte Tabellen:** WordPress-Tabellen erhalten im Hauptinhalt und
  in Zusatzfenstern sichtbare Zelllinien, Kopfzeilen und eine horizontal
  nutzbare Darstellung auf kleinen Bildschirmen.
- **Vollständige Farbanpassung:** Die gewählte Hauptfarbe wird einheitlich auf
  Fensterrahmen, Links, Größen-Griffe und weitere Oberflächenelemente
  angewendet. Vorbereitete Bilddateien bleiben erwartungsgemäß unverändert.
- **Sicherer Kapitelabstand:** Die Kapitelliste misst die tatsächliche
  Oberkante des unteren Linkmenüs. Bei knappem Platz werden Lektionenknoten und
  Kapitel gemeinsam verschoben, sodass auch eine variable Zahl von Kapiteln
  das Menü nicht überdeckt.

## Daten und Kompatibilität

- Die neue Zusatzinhalt-Art wird durch das Plugin registriert; eine manuelle
  Datenmigration ist nicht erforderlich.
- Bestehende Beiträge, Seiten, Themen, Glossarbegriffe und Einstellungen
  bleiben erhalten.
- WordPress 7.0 oder neuer und PHP 8.3 oder neuer bleiben Voraussetzung.
- Plugin und Theme müssen gemeinsam auf 2.3.0 aktualisiert werden.

## Prüfung

Die lokale Prüfkette umfasst zusätzlich die Registrierung, Bearbeitung,
Veröffentlichung und REST-Ausgabe der Zusatzinhalte, die Blockeinbindung,
Größenbegrenzungen und automatischen Vorschauen. Die endgültige
Paketinstallation auf der geschützten PTU wurde erfolgreich durchgeführt;
Plugin, Theme, Datenbank und Trennung von der Produktivseite wurden bestätigt.

## 2.2.1 – 2026-09-20

- Das Glossarportal besitzt nun unabhängig von normalen Seiteneinstellungen
  immer einen Größenregler.
- Kapitelbeschriftungen bleiben oberhalb des unteren Linkmenüs.
- Glossarhinweise funktionieren bei jedem erneuten Mouseover; der Fokus nach
  dem Schließen eines Glossarfensters öffnet keinen Hinweis ungewollt erneut.
- Ein Klick auf das Zentrum beendet auch den Lektionsfokus und lässt das
  Zentrum wieder in den Graphen zurückkehren.
- Medienfenster erzeugen keine zusätzlichen Verlaufsschritte mehr; das
  Lektionsfenster schließt deshalb mit einem einzigen Klick und stellt keine
  ältere Kapitelansicht wieder her.

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
