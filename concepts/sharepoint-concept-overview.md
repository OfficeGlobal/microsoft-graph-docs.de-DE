# <a name="sharepoint-sites-and-content-api-overview"></a>Übersicht über SharePoint-Websites und die Inhalts-API

SharePoint ist Ihr mobiles, intelligentes Intranet. Mit SharePoint können Benutzer Inhalte. Wissen und Anwendungen freigeben und verwalten, um Gruppenarbeit zu stärken, Informationen zu finden und in der Organisation zusammenzuarbeiten. In Microsoft Graph können Sie die REST-API für SharePoint verwenden, um Ihre Lösungen in SharePoint-Websites und -Inhalte zu integrieren.

## <a name="why-integrate-with-sharepoint-sites-and-content"></a>Warum die Integration in SharePoint-Websites und -Inhalte?

SharePoint-Websites unterstützen die Kommunikation und Zusammenarbeit im Team. Office 365-Gruppen, Microsoft Teams und Portale basieren alle auf SharePoint, Sie können daher Microsoft Graph verwenden, um auf Daten zuzugreifen, unabhängig davon, wo diese gespeichert werden. Verwenden Sie die SharePoint-API in Microsoft Graph für den Zugriff auf:

- Teamwebsites, die die Inhalte speichern, an denen Benutzer mit ihren Kollegen zusammenarbeiten.
- Kommunikationswebsites und Portale, in denen Benutzer vielfältige Inhaltsseiten veröffentlichen, die in der gesamten Organisation freigegeben werden sollen.

### <a name="unleash-your-data-with-sharepoint-lists"></a>Nutzen von Daten mit SharePoint-Listen

[Lists][list] sind die Grundlage für die Datenspeicherung in SharePoint.
[Create lists][create] zum Speichern einer Vielzahl von Unternehmensdaten, von einer einfachen Kundenkontaktliste hin zu einer benutzerdefinierten Unternehmensanwendung, bereitgestellt von PowerApps.
Bei Verwendung von [Spalten][] zum Definieren Ihres Schemas, kann SharePoint die Integrität Ihrer Daten schützen und auch Funktionen für eine umfassende Indizierung, Abfragen und Suche aktivieren.

### <a name="bring-the-power-of-lists-to-your-teams-files"></a>Erweitern der Leistungsfähigkeit von Listen auf Dateien Ihres Teams

SharePoint speichert Dateien in einem speziellen [Listentyp][], der als Dokumentbibliothek bezeichnet wird.
Sie können die [OneDrive-API][] zum Arbeiten mit einer Bibliothek als [Laufwerk][] verwenden oder die SharePoint-API zum Arbeiten damit als [Liste][].
Genau wie eine normale Liste können Sie das Schema einer Dokumentbibliothek so erweitern, dass Ihre Unternehmensanforderungen mit benutzerdefinierten Spalten unterstützt werden.

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a>Erweitern Sie Ihre App mit den SharePoint-Intranetdaten Ihrer Benutzer

Mit Microsoft Graph können Sie die wichtigsten Daten Ihrer Benutzer innerhalb Ihrer App anzeigen.
Aktualisieren Sie die Inhalte regelmäßig, indem Sie die Liste [abfragen][], in der die Daten Ihrer Benutzer gespeichert sind.
[Erstellen Sie][] eigene Listen für Ihre App und lassen Sie Benutzer auf Ihre daten in anderen SharePoint-Oberflächen zugreifen, oder blenden Sie Elemente aus.

### <a name="use-microsoft-graph-to-extend-sharepoint"></a>Verwenden von Microsoft Graph zum Erweitern von SharePoint

SharePoint bietet als Plattform verschiedene Modelle für die Erweiterung und Integration:

- Das [SharePoint Framework][] bietet eine Möglichkeit zum Erstellen von Webparts mithilfe von clientseitigen Technologien und Open Source-Tools, die auf SharePoint-Seiten gehostet werden können.
- [SharePoint-Add-Ins][] sind eigenständige Erweiterungen, die einer SharePoint-Website hinzugefügt werden können, ohne dass benutzerdefinierter Code auf dem Server ausgeführt werden muss.

Wenn die App innerhalb einer SharePoint-Seite ausgeführt wird, können Sie problemlos Microsoft Graph verwenden, um auf die Daten über Office 365 hinweg zuzugreifen.

Weitere Details zu diesen Modellen finden Sie im [SharePoint Dev Center][] oder in den [SharePoint Developer-Dokumenten][].

## <a name="next-steps"></a>Nächste Schritte

Erste Schritte mit SharePoint in Microsoft Graph, indem Sie mehr über das [Arbeiten mit Websites][SharePoint] erfahren.

[list]: ../api-reference/v1.0/resources/list.md
[columns]: ../api-reference/v1.0/resources/columndefinition.md
[list type]: ../api-reference/v1.0/resources/listinfo.md
[create]: ../api-reference/v1.0/api/list_create.md
[querying]: ../api-reference/v1.0/api/listitem_get.md
[drive]: ../api-reference/v1.0/resources/drive.md

  [OneDrive-API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive
[SharePoint Framework]: https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview
[SharePoint-Add-Ins]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint Dev Center]: https://developer.microsoft.com/sharepoint
[SharePoint Developer-Dokumente]: http://aka.ms/spdev-docs
[SharePoint]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/sharepoint
