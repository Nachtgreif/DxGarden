# DxGarden

Dieses öffentliche Repository ist der offizielle Veröffentlichungs- und
Update-Kanal für DxGarden.

DxGarden besteht aus zwei gemeinsam versionierten WordPress-Paketen:

- `dxgarden-core-<Version>.zip` – Plugin **DxGarden Core**
- `dxgarden-<Version>.zip` – Theme **DxGarden**

Geprüfte Installationsdateien stehen unter **Releases** bereit. WordPress liest
die aktuelle Version aus [`update.json`](update.json) und prüft jedes Paket vor
der Installation anhand seiner veröffentlichten SHA-256-Prüfsumme.

Dieses Repository enthält bewusst nicht den privaten Entwicklungsquellstand.
Es dient ausschließlich der Verteilung geprüfter Fassungen und ihrer
Update-Metadaten.

## Kompatibilität

- WordPress 7.0 oder neuer
- PHP 8.3 oder neuer

Die praktische Gegenprüfung mit weiteren Screenreadern neben der vorbereiteten
Linux-/Orca-Umgebung bleibt als offener Kompatibilitätstest dokumentiert.
