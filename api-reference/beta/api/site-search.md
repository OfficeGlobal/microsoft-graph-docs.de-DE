---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Suchen von SharePoint-Websites nach Stichwort
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ee4aa139508e6a523ea1858c6b0598a5b8aaf9b5
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480754"
---
# <a name="search-for-sites"></a>Nach Websites suchen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können in einem gesamten SharePoint-Mandanten nach [Websites][] suchen, die den angegebenen Schlüsselwörtern entsprechen.

[Websites]: ../resources/site.md

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)
|:--------------------------------------|:-------------------------------------
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | Sites.Read.All, Sites.ReadWrite.All
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt
|Anwendung                            | Sites.Read.All, Sites.ReadWrite.All

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET https://graph.microsoft.com/beta/sites?search={query}
```

## <a name="response"></a>Antwort

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.site)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteB"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
    "Error: /api-reference/beta/api/site-search.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
