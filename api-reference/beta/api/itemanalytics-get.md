---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Analysen abrufen
localization_priority: Normal
ms.openlocfilehash: d1f6b255747cffe7fdccb5d098e73a56151b6245
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516259"
---
# <a name="get-analytics"></a>Analysen abrufen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rufen Sie [ItemAnalytics][] über die Ansichten, die unter diese Ressource durchgeführt wurde.
Die **ItemAnalytics** Ressource ist eine bequeme Möglichkeit zum Abrufen der Aktivität Statistik für `allTime` und die `lastSevenDays`.
Verwenden Sie für einen benutzerdefinierten Zeitbereich oder Intervall [GetActivitiesByInterval][] API.

>**Hinweis:** Die Ressource **ItemAnalytics** ist noch nicht in allen [nationalen Bereitstellungen](/graph/deployments)verfügbar.

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)
|:--------------------------------------|:-------------------------------------
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt
|Anwendung                            | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a>Beispiel

#### <a name="request"></a>Anforderung

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a>Antwort

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
