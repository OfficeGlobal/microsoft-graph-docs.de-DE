# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a>Arbeiten mit SharePoint-Websites in Microsoft Graph

Die SharePoint-API in Microsoft Graph unterstützt die folgenden wesentlichen Szenarios:

* Zugriff auf SharePoint-**Websites**, **-Listen** und **-Laufwerke** (Dokumentbibliotheken)
* Schreibgeschützte Unterstützung für **Website**-Ressourcen (keine Möglichkeit zum Erstellen neuer Websites)
* Lese-/ Schreibzugriff-Unterstützung für **-Listen**, **listItems** und **driveItems**
* Adressierung von Ressourcen nach SharePoint-ID, URL oder relativem Pfad

Die SharePoint-API macht drei wichtige Ressourcentypen verfügbar:

* [Site](site.md) _ (Objekt auf oberster Ebene)_
* [List](list.md)
* [ListItem](listitem.md)

Es folgt ein Beispiel für eine listItem-Ressource:

```json
{
  "fields": {
    "Title": "Access card",
    "Employee": "Ryan Gregg",
    "EmployeeId": "10",
    "CardSerial": "01235492",
    "Alias": "RGregg",
    "ID": 1,
    "ContentType": "Item",
    "Modified": "2016-09-19T23:15:25-07:00",
    "Created": "2016-09-19T23:15:25-07:00"
  },
  "createdBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "createdDateTime": "2016-09-20T06:15:25Z",
  "eTag": "48e941c3-9515-4c48-9760-c07c90c79d48,1",
  "id": "4",
  "lastModifiedBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "lastModifiedDateTime": "2016-09-20T06:15:25Z",
}
```

Ressourcen legen Daten auf drei verschiedene Arten offen:

* _Eigenschaften_ (wie **id** und **name**) legen einfache Werte offen.
* _Facets_ (wie **fields** und **createdBy**) legen komplexe Werte offen.
* _References_ (wie **items**) verweisen auf Sammlungen anderer Ressourcen.

Sie können Sie Referenzen in der URL mit dem _expand_-Abfrageparameter erweitern, z. B. `?expand=fields`.
Sie können bestimmte Eigenschaften und Facets mit dem _select_ Abfrageparameter abrufen, z. B. `?select=id,name`.
Standardmäßig werden die meisten Eigenschaften und Facets zurückgegeben, wohingegen alle Referenzen ausgeblendet werden.
Aus Leistungsgründen wird empfohlen, dass Sie _select_ und _expand_ nur für die Daten angeben, an denen Sie interessiert sind.

## <a name="sharepoint-api-root-resources"></a>SharePoint-API-Stammressourcen

Die folgenden Beispiele sind relativ zu `https://graph.microsoft.com/v1.0`.

| Pfad                                   | Beschreibung
|:---------------------------------------|:------------------------------------
| /sites/root                            | Standardmäßige [Website][] der Organisation
| /sites/{site-id}                       | Zugriff auf eine bestimmte [Website][] anhand ihrer ID
| /sites/{site-id}/drive                 | Zugriff auf das standardmäßige [Laufwerk](drive.md) (Dokumentbibliothek) für die angegebene [Website][]
| /sites/{site-id}/drives                | Aufzählung der [Laufwerke](drive.md) (Dokumentbibliotheken) unter der [Website][]
| /sites/{site-id}/sites                 | Aufzählung der Unterwebsites unter der [site][]
| /sites/{site-id}/lists                 | Aufzählung der [lists](list.md) unter der [site](site.md)
| /sites/{site-id}/lists/{list-id}/items | Aufzählung der [listItems](listitem.md) unter der [list](list.md)
| /groups/{group-id}/sites/root          | Zugriff auf die Teamweb[site][] einer Gruppe

Websites können auch anhand des Pfads adressiert werden, indem der SharePoint-Hostname gefolgt von einem Doppelpunkt und dem relativen Pfad zur Website verwendet wird. Sie können optional wieder zur Adressierung des Ressourcenmodells übergehen, indem Sie einen Doppelpunkt am Ende einfügen.

| Path                                           | Beschreibung
|:-----------------------------------------------|:-----------------------------------
| /sites/contoso.sharepoint.com:/teams/hr        | Die Website, die https://contoso.sharepoint.com/teams/hr zugeordnet ist
| /sites/contoso.sharepoint.com:/teams/hr:/drive | Zugriff auf das standardmäßige [Laufwerk](drive.md) für diese Website

## <a name="note-for-existing-sharepoint-developers"></a>Hinweis für bestehende SharePoint-Entwickler

Zwischen der Microsoft Graph-SharePoint-API und den CSOM-APIs bestehen einige wesentliche Unterschiede.
Die [site][]-Ressource ist `SPWeb` zugeordnet.
Die Stammweb[site][] (`SPWeb`) in einer Websitesammlung verfügt über ein [siteCollection](sitecollection.md)-Facet, das Informationen über `SPSite` enthält.
Da IDs für Websites nur innerhalb einer Websitesammlung eindeutig sind, müssen zur Adressierung einer Website nach ID sowohl die Websitesammlungs-ID als auch die Website-ID angegeben werden.

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id},{spweb-id}/
```
Eine URL, die nur mit dem Hostnamen gebildet wird, verweist auf die Stammwebsite (`SPWeb`) in der Standard-Websitesammlung.

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname}
```

Eine URL, die nur mit dem Hostnamen und der Websitesammlungs-ID (`SPSite`) gebildet wird, verweist auf die Stammwebsite (`SPWeb`) in der angegebenen Websitesammlung.

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id}
```

[site]: site.md
[list]: list.md
[drive]: drive.md
[siteCollection]: siteCollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->
