---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePoint-Website nach Pfad abrufen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: afded48114342e8bf5eb76d25f1361f67686af54
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936186"
---
# <a name="get-a-site-resource-by-path"></a>Site-Ressource nach Pfad abrufen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Dient zum Abrufen der Eigenschaften und Beziehungen einer [site][]-Ressource. Eine **site**-Ressource stellt eine Teamwebsite in SharePoint dar.

[site]: ../resources/site.md

Zusätzlich zum Abrufen einer [Website nach ID](site-get.md) können Sie eine Website basierend auf dem serverrelativen URL-Pfad abrufen.

* Hostname der Websitesammlung (contoso.sharepoint.com)
* Websitepfad relativ zum Hostnamen des Servers

Es gibt auch einen reservierten Websitebezeichner, `root`, der immer auf die Stammwebsite für ein angegebenes Ziel verweist, wie folgt:

* `/sites/root`: Der Stammwebsite des Mandanten.
* `/groups/{group-id}/sites/root`: Die Teamwebsite der Gruppe.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

So greifen Sie mit einem relativen Pfad auf die SharePoint-Stammwebsite zu:

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a>Antwort

Diese Methode gibt eine [site][]-Ressource für die Website zurück, auf die vom eindeutigen Bezeichner verwiesen wird.

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "owner": {
    "user": { 
      "displayName": "Daron Spektor",
      "id": "5280E7FE-DC7A-4486-9490-E790D81DFEB3"
    }
  },
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by path"
} -->
