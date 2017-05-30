# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a>Arbeiten mit SharePoint-Websites in Microsoft Graph

Die SharePoint-API in Microsoft Graph unterstützt die folgenden wesentlichen Szenarios:

* Zugriff auf SharePoint-**Websites** und -**Laufwerke** (Dokumentbibliotheken)
* Schreibgeschützte Unterstützung für **Website**-Ressourcen (keine Möglichkeit zum Erstellen neuer Websites)
* Lese-/Schreibunterstützung für **driveItems**
* Adressierung von Ressourcen nach SharePoint-ID, URL oder relativem Pfad

## <a name="sharepoint-api-root-resources"></a>SharePoint-API-Stammressourcen

Die folgenden Beispiele sind relativ zu `https://graph.microsoft.com/v1.0`.

| Pfad                                   | Beschreibung
|:---------------------------------------|:------------------------------------
| /sites/root                            | Standardmäßige [Website][] der Organisation
| /sites/{site-id}                       | Zugriff auf eine bestimmte [Website][] anhand ihrer ID
| /sites/{site-id}/drive                 | Zugriff auf das standardmäßige [Laufwerk](drive.md) (Dokumentbibliothek) für die angegebene [Website][]
| /sites/{site-id}/drives                | Aufzählung der [Laufwerke](drive.md) (Dokumentbibliotheken) unter der [Website][]
| /sites/{site-id}/sites                 | Aufzählung der Unterwebsites unter der [Website][]
| /groups/{group-id}/sites/root          | Zugriff auf die Team[website][] einer Gruppe

Websites können auch anhand des Pfads adressiert werden, indem der SharePoint-Hostname gefolgt von einem Doppelpunkt und dem relativen Pfad zur Website verwendet wird. Sie können optional wieder zur Adressierung des Ressourcenmodells übergehen, indem Sie einen Doppelpunkt am Ende einfügen.

| Pfad                                           | Beschreibung
|:-----------------------------------------------|:-----------------------------------
| /sites/contoso.sharepoint.com:/teams/hr        | Die Website, die https://contoso.sharepoint.com/teams/hr zugeordnet ist
| /sites/contoso.sharepoint.com:/teams/hr:/drive | Zugriff auf das standardmäßige [Laufwerk](drive.md) für diese Website

## <a name="note-for-existing-sharepoint-developers"></a>Hinweis für bestehende SharePoint-Entwickler

Zwischen der Microsoft Graph-SharePoint-API und den CSOM-APIs bestehen einige wesentliche Unterschiede. Die [site][]-Ressource ist `SPWeb` zugeordnet. Die Stammweb[site][] (`SPWeb`) in einer Websitesammlung verfügt über ein [siteCollection](sitecollection.md)-Facet, das Informationen über `SPSite` enthält. Da IDs für Websites nur innerhalb einer Websitesammlung eindeutig sind, müssen zur Adressierung einer Website nach ID sowohl die Websitesammlungs-ID als auch die Website-ID angegeben werden.

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
