# <a name="sharepoint-site-usage-reports"></a>Verwendungsberichte für SharePoint-Website

Sie können die Verwendungsberichte für die SharePoint-Website nutzen, um eine allgemeine Übersicht über den Nutzungswert von SharePoint hinsichtlich der Gesamtzahl der Dateien, die Benutzer in SharePoint-Websites speichern, der Anzahl der aktiv genutzten Dateien und des Speicherplatzes, der für all diese Websites verbraucht wird, zu erhalten. Sie können auch einen Drilldown ausführen, um Trends zu erfassen und Details zu den einzelnen Websites zu erhalten.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Websiteverwendung](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp | Beschreibung                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Websitedetails abrufen](../api/reportroot_getsharepointsiteusagedetail.md) | Stream      | Abrufen von Details zu SharePoint-Websiteverwendung. |
| [Dateianzahl abrufen](../api/reportroot_getsharepointsiteusagefilecounts.md) | Stream      | Rufen Sie die Gesamtzahl der Dateien auf allen Websites und die Anzahl der aktiven Dateien ab. Eine Datei (Benutzer oder System) wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde. |
| [Websiteanzahl abrufen](../api/reportroot_getsharepointsiteusagesitecounts.md) | Stream      | Rufen Sie die Gesamtzahl der Dateien auf allen Websites und die Anzahl der aktiven Dateien ab. Eine Datei (Benutzer oder System) wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde. |
| [Speicher abrufen](../api/reportroot_getsharepointsiteusagestorage.md) | Stream      | Erhalten Sie eine Übersicht über den im Berichtszeitraum zugewiesenen und belegten Speicherplatz. |
| [Seiten abrufen](../api/reportroot_getsharepointsiteusagepages.md) | Stream      | Rufen Sie die Anzahl der angezeigten Seiten aller Websites ab. |
