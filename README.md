# EAD(DDB) Beispiel- und Schemadateien

In diesem Repository finden sich die offiziellen XML-Schema-Dateien sowie Beispieldateien zu EAD(DDB) in der aktuellen Version 1.2.

Die Schemata und Beispiele sind abwärtskompatibel zu EAD(DDB) 1.0 bis 1.1, weshalb die hier vorliegende Versionen auch für Instanzen des älteren Formats verwendet werden können. Deshalb werden die älteren Revisionen hier nicht hinterlegt.

## Struktur des Repositories

Im Unterordner `ead_ddb/1.2/example` finden sich Beispieldateien, darunter:

- Minimalbeispiele, welche lediglich die Pflichtbelegung von Elemente und Attributen beinhalten.
- Maximalbeispiele, welche alle möglichen Elemente und Attribute enthalten. 
- Optimalbeispiele, welche die für die Darstellung im DDB- und Archivportal sinnvolle Belegung wiedergibt.
- Neben der EAD-Beispielen wird auch auch ein Minimal- und Maximalbeispiel für das archivische METS/MODS-Profil mit aufgenommen. So befüllte METS/MODS-Dateien können verwendet werden, um den DFG-Viewer zu bespielen und z.B. in DDB bzw. Archivportal-D verwenden zu können.

Im Unterordner `ead_ddb/1.2/schema` finden Sie XML-Schema-Dateien zur Validierung von EAD(DDB)-Dateien. Vorzugsweise sollten die Schemata nach der Schema-Definition 1.1 (`..._XSD1.1.xsd`) verwendet werden, da diese eine wesentlich genauere Abprüfung der Validierungsregeln erlauben. Für XML-Parser, die XSD 1.1 nicht unterstützen, werden die Schemata auch in Version 1.0 bereitgestellt.

## Errata

Über Verbesserungsvorschläge bzw. Fehlerberichte freuen wir uns. Diese können Sie unter [Issues](https://github.com/Deutsche-Digitale-Bibliothek/ddb-metadata-ead/issues) anlegen.

## Changelog
- 2019-07-15: EAD(DDB) 1.2 (Bugfix): Abprüfung der korrekten Findbuch-Struktur (Bestandsdatensatz als oberster c-Knoten). Dateien mit falscher Struktur wurden nicht weiter validiert und fälschlicherweise als valide deklariert.
- 2019-04-01: Erste Veröffentlichung der Schemata und Beispieldateien zu EAD(DDB) 1.2.

## Weiterführende Informationen

Eine ausführliche Dokumentation folgt in Kürze und wird dann hier verlinkt.

Weitere Informationen zu EAD(DDB) auf den Seiten des [Landesarchivs Baden-Württemberg](https://www.landesarchiv-bw.de/ead ).