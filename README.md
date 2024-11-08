# EAD(DDB) Beispiel- und Schemadateien

In diesem Repository finden sich die offiziellen XML-Schema-Dateien sowie Beispieldateien zu EAD(DDB) in der aktuellen Version 1.2.

Die Schemata und Beispiele sind abwärtskompatibel zu EAD(DDB) 1.0 bis 1.1, weshalb die hier vorliegenden Versionen auch für Instanzen des älteren Formats verwendet werden können. Deshalb werden die älteren Revisionen hier nicht hinterlegt.

## Struktur des Repositories
### EAD(DDB)
Im Unterordner `ead_ddb/1.2/example` finden sich Beispieldateien, darunter:

- Minimalbeispiele, welche lediglich die Pflichtbelegung von Elementen und Attributen beinhalten.
- Maximalbeispiele, welche alle möglichen Elemente und Attribute enthalten. 
- Optimalbeispiele, welche die für die Darstellung in DDB- und Archivportal sinnvolle Belegung wiedergibt.
- Neben den EAD-Beispielen wird auch ein Minimal- und Maximalbeispiel für das archivische METS/MODS-Profil mit aufgenommen. So befüllte METS/MODS-Dateien können verwendet werden, um den DFG-Viewer zu bespielen und z.B. in DDB bzw. Archivportal-D verwenden zu können.

Im Unterordner `ead_ddb/1.2/schema` finden Sie XML-Schema-Dateien zur Validierung von EAD(DDB)-Dateien. Vorzugsweise sollten die Schemata nach der Schema-Definition 1.1 (`..._XSD1.1.xsd`) verwendet werden, da diese eine wesentlich genauere Abprüfung der Validierungsregeln erlauben. Für XML-Parser, die XSD 1.1 nicht unterstützen, werden die Schemata auch in Version 1.0 bereitgestellt.

### EAD(DDB)-WGM
Im Unterordner `ead_ddb_wgm/1.2/example` findet sich eine Findbuch-Beispieldatei für das EAD(DDB)-WGM-Anwendungsprofil zur Verwendung im [Themenportal Wiedergutmachung](https://www.archivportal-d.de/themenportale/wiedergutmachung). 
Die Beispieldatei basiert auf der jeweils aktuellen Version von EAD(DDB) 1.2.

Eine XML-Schema-Datei zur Validierung von Findbüchern im EAD(DDB)-WGM-Format finden Sie im Unterordner `ead_ddb_wgm/1.2/schema`. Zur Validierung von Tektonik-Dateien kann das reguläre EAD(DDB)-Schema verwendet werden.

Weitere Informationen zum EAD(DDB)-WGM-Anwendungsprofil finden sich in der [Dokumentation](https://wiki.deutsche-digitale-bibliothek.de/pages/viewpage.action?pageId=126518213).

## Errata

Über Verbesserungsvorschläge bzw. Fehlerberichte freuen wir uns. Diese können Sie unter [Issues](https://github.com/Deutsche-Digitale-Bibliothek/ddb-metadata-ead/issues) anlegen.

## Changelog
- 2024-11-08: XML-Schema für EAD(DDB)-WGM: Vokabular für Schadensarten und Staatsangehörigkeit um fehlenden Wert ergänzt.
- 2024-11-04: Beispieldatei und XML-Schema für EAD(DDB)-WGM Version 1.2 veröffentlicht.
- 2024-01-16: Beispieldatei für EAD(DDB)-WGM - fehlerbereinigte und erweiterte Version 1.1 veröffentlicht. Die bisherige Version 1.0 wird nicht mehr gepflegt.
  - Erklärende Kommentare mit Verweis auf Feldnummern des Metadatenkatalogs ergänzt
  - Vorauswahl-Wert für das Feld Archivalientyp (`//c/did/physdesc/genreform`) festgelegt
  - Feld 31 analog zu natürlichen Personen (die sowohl „antragstellend“ als auch „verfolgt“ sein können) offener betitelt
  - Feld 47, 48 und 49 hinzugefügt
  - Feld 50, 51, 60 spezifiziert
  - Feld 56 entsprechend dem Metadatenkatalog in „abweichende Laufzeit“ geändert
  - Feld 59 entsprechend dem Metadatenkatalog in „Vorsignaturen“ geändert
- 2013-12-14: Beispieldatei für EAD(DDB)-WGM 1.0 – Zulässige Werte des Feldes "Rolle" korrigiert.
- 2023-12-12: Beispieldatei für EAD(DDB)-WGM 1.0 hinzugefügt. Link zur Dokumentation in Beispieldateien für EAD(DDB) 1.2 ergänzt.
- 2020-02-04: Beispieldateien und Schemata für EAD(DDB) 1.1 zur Dokumentation hinterlegt. [Neue Dokumentation](https://wiki.deutsche-digitale-bibliothek.de/pages/viewpage.action?pageId=19010180) verlinkt.
- 2019-11-28: EAD(DDB) 1.2 Findbuch-XSD (Bugfix): `//c[@level="file"]/did/unitid` und `/ead/archdesc/otherfindaid` nicht als Pflichtelement behandeln.
- 2019-07-15: EAD(DDB) 1.2 (Bugfix): Abprüfung der korrekten Findbuch-Struktur (Bestandsdatensatz als oberster `c`-Knoten). Dateien mit falscher Struktur wurden nicht weiter validiert und fälschlicherweise als valide deklariert.
- 2019-04-01: Erste Veröffentlichung der Schemata und Beispieldateien zu EAD(DDB) 1.2.

## Weiterführende Informationen

Weitere Informationen zu EAD(DDB) sowie eine ausführliche Dokumentation finden Sie [hier](https://wiki.deutsche-digitale-bibliothek.de/pages/viewpage.action?pageId=19010180).
