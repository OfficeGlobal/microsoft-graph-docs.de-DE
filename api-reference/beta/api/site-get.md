---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePoint-Website abrufen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 69845652cef0f726ae466a093bf504320c0fdd50
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508573"
---
# <a name="get-a-site-resource"></a>Site-Ressource abrufen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dient zum Abrufen der Eigenschaften und Beziehungen einer [site][]-Ressource. Eine **site**-Ressource stellt eine Teamwebsite in SharePoint dar.

[site]: ../resources/site.md

Eine **site**-Ressource wird durch einen eindeutigen Bezeichner adressiert; dies ist eine aus den folgenden Werten zusammengesetzte ID:

* Hostname der Websitesammlung (contoso.SharePoint.com)
* Eindeutige ID der Websitesammlung (GUID)
* Eindeutige ID der Website (GUID)

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

## <a name="get-the-tenants-root-site"></a>Abrufen der Stammwebsite eines Mandanten

So greifen Sie innerhalb eines Mandanten auf die SharePoint-Stammwebsite zu:

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a>Über eine serverrelative URL auf eine Website zugreifen

Wenn Sie über die serverrelative URL für eine **site**-Ressource verfügen, können Sie eine Anforderung wie folgt erstellen:

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a>Auf die Teamwebsite einer Gruppe zugreifen

So greifen Sie auf die Teamwebsite für eine  Gruppe zu:

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a>Antwort

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID",
  "suppressions": [
    "Error: /api-reference/beta/api/site-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
