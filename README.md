# DxGarden

Dieses öffentliche Repository ist der offizielle Veröffentlichungs- und
Update-Kanal für DxGarden.

DxGarden besteht aus zwei gemeinsam versionierten WordPress-Paketen:

- `dxgarden-core-<Version>.zip` – Plugin **DxGarden Core**
- `dxgarden-<Version>.zip` – Theme **DxGarden**

Geprüfte Installationsdateien stehen unter **Releases** bereit. WordPress liest
die aktuelle Version aus [`update.json`](update.json) und prüft jedes Paket vor
der Installation anhand seiner veröffentlichten SHA-256-Prüfsumme.

Aktuelle geprüfte Fassung: [DxGarden 1.1.3](https://github.com/Nachtgreif/DxGarden/releases/tag/dxgarden-v1.1.3)

Die Versionsschritte 1.1.0 bis 1.1.2 sind unter **Releases** mit ihren
ursprünglichen Angaben und Prüfsummen dokumentiert. Ihre veralteten
Installationspakete werden nicht erneut angeboten; installierbare Dateien gibt
es ausschließlich für die aktuelle Fassung.

Dieses Repository enthält bewusst nicht den privaten Entwicklungsquellstand.
Es dient ausschließlich der Verteilung geprüfter Fassungen und ihrer
Update-Metadaten.

## Entwicklung und Rückmeldungen

- [Öffentliche Roadmap](ROADMAP.md) – Vorschläge und angenommene Änderungen
- [Changelog](CHANGELOG.md) – bereits umgesetzte Produktänderungen
- [Issues](https://github.com/Nachtgreif/DxGarden/issues) – Fehler melden oder eine Änderung vorschlagen
- [Nächste Hauptversion 2.0.0](https://github.com/Nachtgreif/DxGarden/milestone/1) – WordPress-nahe Konsolidierung und öffentlich eingeplante Änderungen

Vorschläge anderer Nutzer und direkte Projektentscheidungen werden auf
derselben Roadmap geführt, bleiben aber über ihre Herkunft gekennzeichnet.
Details zum Ablauf stehen in den [Mitwirkungsregeln](CONTRIBUTING.md).

## Kompatibilität

- WordPress 7.0 oder neuer
- PHP 8.3 oder neuer

Die praktische Gegenprüfung mit weiteren Screenreadern neben der vorbereiteten
Linux-/Orca-Umgebung bleibt als offener Kompatibilitätstest dokumentiert.
