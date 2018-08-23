# <a name="excel-workbooks-and-charts-api-overview"></a>Übersicht über Excel-Arbeitsmappen und die Diagramme-API

Excel ist eine unentbehrliches Produktivitätswerkzeug. Benutzer in allen Branchen und aller Hierarchieebenen nutzen das Programm als Werkzeug zum Speichern, Nachverfolgen und Bearbeiten aller Arten von Daten. Excel wird für alle möglichen Aufgaben verwendet, von der einfachen Aufgabennachverfolgung und Datenverwaltung bis hin zu komplexen Berechnungen und professioneller Berichterstellung. Sie können die Excel-REST-API in Microsoft Graph verwenden, um den Wert Ihrer Daten, Berichte und Dashboards noch zu erhöhen.

## <a name="why-integrate-with-excel"></a>Vorteile der Integration mit Excel

Sie können Microsoft Graph verwenden, um es Web- und Mobilanwendungen zu ermöglichen, in OneDrive, SharePoint oder anderen unterstützten Speicherplattformen gespeicherte Excel-Arbeitsmappen zu lesen und zu bearbeiten.

### <a name="perform-calculations"></a>Ausführen von Berechnungen

Benutzer schätzen die Einfachheit, mit der sie umfassende und komplexe Berechnungen in Excel ausführen können. Sie können nun auf das leistungsfähige Rechenmodul in Excel zugreifen und sofortige Ergebnisse erhalten. So kann ein Hypothekenrechner beispielsweise die RMZ-Funktion von Excel nutzen, indem er einen einfachen API-Aufruf durchführt, der Kapital, Zins und Anzahl der Zahlungen enthält. Excel führt alle schwierige Arbeiten durch und gibt die monatliche Zahlung sofort zurück. Derzeit sind mehr als 300 Funktionen für Excel-Arbeitsblätter verfügbar, sodass Sie die gesamte Palette der Formeln nutzen können, die von Excel unterstützt werden. Komplexe Geschäftsmodellen müssen nicht wiederholt neu erstellt werden. Entwickler können Excel so programmieren, dass diese Berechnungen sofort ausgeführt werden die Ergebnisse mit einfachen API-Aufrufen abrufen.

### <a name="generate-reports-and-analyze-results"></a>Generieren von Berichten und Analysieren der Ergebnisse

Excel ist ein flexibles Berichterstellungs- und Analysetool für einfache Datentabellen bis hin zu komplexen professionellen Dashboards. Sie haben heute vollen Zugriff auf alle Excel-Berichterstellungsfunktionen, indem wir Ihnen Excel als Onlinedienst für die Berichterstellung in Office 365 zur Verfügung stellen. Stellen Sie sich alle Szenarien der Berichterstellung vor, die Benutzer heute erstellen und auf die sie sich verlassen. Diese sind nun in einer anpassbaren App verfügbar, sodass Sie professionelle Diagramme erstellen oder umfangreiche Datensätze intelligent analysieren können. Excel ist nahtlos in diese benutzerdefinierten Oberflächen integriert.

### <a name="store-and-track-data"></a>Speichern und Nachverfolgen von Daten

Excel ist auch ein hervorragendes Tool zum Speichern und Nachverfolgen von Daten. Wenn Ihre Daten in einer Arbeitsmappe gespeichert sind, steht diese Daten jeder App zur Verfügung, die in Office 365 integriert werden kann. Die Inhalte können von benutzerdefinierten Lösungen gelesen werden, und diese Lösungen können Excel zum Speichern der Daten nutzen.

>**Hinweis:** Die Excel-REST-API unterstützt nur Arbeitsmappen, die als Office Open XML-Dateien formatiert sind (Dateien mit der Erweiterung `.xlsx`). Arbeitsmappen mit der Erweiterung `.xls` werden nicht unterstützt. 

### <a name="using-the-excel-rest-api"></a>Verwenden der Excel-REST-API
Sie können Microsoft Graph verwenden, um es Web- und Mobilanwendungen zu ermöglichen, in OneDrive, SharePoint oder anderen unterstützten Speicherplattformen gespeicherte Excel-Arbeitsmappen zu lesen und zu bearbeiten. Die `Workbook`- (bzw. Excel-Datei-)Ressource enthält alle anderen Excel-Ressourcen über Beziehungen. Sie können über die Laufwerks-API auf eine Arbeitsmappe zugreifen, indem Sie den Speicherort der Datei in der URL identifizieren. Beispiel:

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`

`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/ `

Sie können auf eine Reihe von Excel-Objekten (wie Tabelle, Bereich oder Diagramm) mithilfe von standardmäßigen REST-APIs zugreifen, um Vorgänge zum Erstellen, Lesen, Aktualisieren und Löschen in der Abeitsmappe durchzuführen.

## <a name="next-steps"></a>Nächste Schritte

* [Verwalten von Sitzungen in Excel mit Microsoft Graph](excel-manage-sessions.md)
* [Schreiben in eine Excel-Arbeitsmappe mit Microsoft Graph](excel-write-to-workbook.md)
* [Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph](excel-use-functions.md)
* [Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph](excel-update-range-format.md)
* [Ein Diagrammbild in Excel mithilfe von Microsoft Graph anzeigen](excel-display-chart-image.md)
* [Verwenden der Excel-REST-API](../api-reference/v1.0/resources/excel.md)
