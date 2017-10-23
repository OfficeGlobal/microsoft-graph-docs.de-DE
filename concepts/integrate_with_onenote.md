# <a name="use-microsoft-graph-to-integrate-with-onenote"></a>Verwenden von Microsoft Graph für die Integration in OneNote

Durch die Integration Ihrer Apps in OneNote können Sie Erfahrungen plattformübergreifend für Millionen von Nutzern weltweit bereitstellen. Mit Microsoft Graph können Sie auf Notizbücher, Abschnitte und Seiten in OneNote-Lösungen zugreifen, um Ihren Benutzern zu helfen, Ideen umzusetzen und Informationen zu ordnen.

## <a name="why-create-onenote-apps"></a>Warum sollte ich OneNote-Apps erstellen?

Sie können Microsoft Graph verwenden, um Notizen, Listen, Bilder, Dateien usw. in OneNote-Notizbüchern zu erstellen und verwalten.

### <a name="collect-and-organize-notes-and-ideas"></a>Erfassen und Organisieren von Notizen und Ideen  
Verwenden Sie OneNote als Hilfsmittel zum Hinzufügen und Ordnen von Benutzerinhalten. Microsoft Graph vereinfacht das Schreiben von Apps, mit denen Studenten Notizen erstellen und recherchieren, Familien Pläne und Ideen teilen oder Einkäufer Bilder freigeben können. Ihre App sammelt die gewünschten Informationen, sendet sie an OneNote und hilft dann bei der Verwaltung dieser Informationen.

### <a name="capture-information-in-many-formats"></a>Erfassen von Informationen in vielen verschiedenen Formaten
Erfassen Sie HML-Code, eingebettete Bilder (aus einer lokalen Quelle oder öffentlichen URL), Videos, Audio, E-Mail-Nachrichten und andere gängige Dateitypen. OneNote kann sogar Webseiten und PDF-Dateien als Snapshots darstellen. Microsoft Graph unterstützt eine Reihe von standardmäßigen HTML- und CSS-Codes für das OneNote-Seitenlayout, sodass Sie Tabellen, Inline-Bilder und einfache Formatierungen verwenden können, um den gewünschten Look zu erzielen. 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a>Verwenden Sie das Ökosystem von OneNote, um Ihre wichtigsten Szenarien zu verbessern.
Probieren Sie andere leistungsfähige Funktionen von OneNote aus. Die OneNote-APIs in Microsoft Graph führen OCR für Bilder aus, unterstützen die Volltextsuche, synchronisieren automatisch Clients, verarbeiten Bilder und extrahieren Visitenkarte sowie Online-Produkt- und Rezeptlisten. Verwenden Sie OneNote als digitalen Erinnerungsspeicher in der Cloud für Notizen und einfache Medien oder als Datenfeed für domänenspezifische Daten. 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a>Millionen von OneNote-Benutzern auf allen wichtigen Plattformen erreichen
Verwenden Sie OneNote, um Ihre App-Nutzung zu steigern. OneNote ist auf neuen Windows-Geräten vorinstalliert und steht für die meisten Plattformen, online und als Bestandteil von Office 365 zur Verfügung. Wenn Sie Apps veröffentlichen, die die funktionsreiche OneNote-Umgebung verwenden, haben Sie Zugriff auf umfassendes plattformübergreifendes Marktpotenzial.

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: https://developer.microsoft.com/en-us/graph/docs/concepts/featured_scenarios. You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a>Wozu kann ich OneNote-APIs in Microsoft Graph verwenden?

Im folgenden werden einige der am häufigsten verwendeten Anfragen für OneNote-Ressourcen vorgestellt.

|Vorgang|URL|
|:--------|:--|
|Abrufen meiner Notizbücher|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|Abrufen meiner Abschnitte|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|Abrufen meiner Seiten|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="explore-the-onenote-apis"></a>Erkunden Sie die OneNote-APIs
Verwenden Sie den [Microsoft Graph-Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer), um die OneNote-APIs mit Ihren eigenen OneNote-Notizbüchern auszuprobieren.

Um OneNote-API-Anrufe über den Graph Explorer auszuführen, wählen Sie **Mehr Beispiele anzeigen** in der Spalte auf der linken Seite. Schalten Sie OneNote über das Menü **Ein**. Zudem müssen Sie die entsprechenden Berechtigungen aktivieren. Wählen Sie unter Ihrem Kontonamen im Menü auf der linken Seite **Berechtigungen ändern**. Weitere Informationen über OneNote-Berechtigungen finden Sie unter [Notizenberechtigungen](permissions_reference.md#notes-permissions).

Hinweise zu den ersten Schritten mit OneNote-APIs in Microsoft Graph finden Sie unter [Referenzinhalte für OneNote](../api-reference/v1.0/resources/onenote.md).

## <a name="see-also"></a>Siehe auch

* [Brandingrichtlinien](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-branding)
* [Abrufen von OneNote-Inhalt und -Struktur](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-get-content)
* [Hinzufügen von Bildern, Videos und Dateien](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files)
* [Erstellen von absolut positionierten Elementen](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)
* [Extrahieren von Daten](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data)
* [Verwenden von Notiztags](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)

