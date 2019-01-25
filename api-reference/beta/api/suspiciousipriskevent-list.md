---
title: Liste suspiciousIpRiskEvents
description: Abrufen einer Liste von Suspiciousipriskevent-Objekten.
localization_priority: Normal
ms.openlocfilehash: 1caad773d401367b93bece5d30191a5c98b7b935
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513802"
---
# <a name="list-suspiciousipriskevents"></a>Liste suspiciousIpRiskEvents

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abrufen einer Liste von Suspiciousipriskevent-Objekten.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | IdentityRiskEvent.Read.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | IdentityRiskEvent.Read.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents
```
## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Arbeitsmappensitzungs-ID  | Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [SuspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) .
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
    {
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:08:35.123512Z",
      "id": "02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:33:49.9516789Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "SuspiciousIpRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "97b7301f-bc05-8e2c-fdfa-2004eb66ff70",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List suspiciousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/suspiciousipriskevent-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
