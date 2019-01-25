---
title: assignLicense
description: Hinzufügen oder Entfernen von Lizenzen für den Benutzer aktivieren oder Deaktivieren der Verwendung von Microsoft-Cloud-angeboten. Beispielsweise eine Organisation kann ein Office 365 Enterprise E3-Abonnement mit 100 Lizenzen verfügen, und diese Anforderung weist eine der Lizenzen, die für einen bestimmten Benutzer. Sie können auch aktivieren und Deaktivieren von bestimmten Pläne ein Abonnement zugeordnet. Weitere Informationen zu Abonnements und Lizenzen finden Sie unter Technet-Artikel.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d15202d24148b2f75bd857500117a4f97b61fe51
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510498"
---
# <a name="assignlicense"></a>assignLicense

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Hinzufügen oder Entfernen von Lizenzen für den Benutzer aktivieren oder Deaktivieren der Verwendung von Microsoft-Cloud-angeboten. Beispielsweise eine Organisation kann ein Office 365 Enterprise E3-Abonnement mit 100 Lizenzen verfügen, und diese Anforderung weist eine der Lizenzen, die für einen bestimmten Benutzer. Sie können auch aktivieren und Deaktivieren von bestimmten Pläne ein Abonnement zugeordnet. Weitere Informationen zu Abonnements und Lizenzen finden Sie unter in diesem [Technet-Artikel](https://technet.microsoft.com/en-us/library/mt765146.aspx).

Wenn die im Verzeichnis Abonnements erhalten möchten, führen Sie eine [GET-Anforderung SubscribedSkus](subscribedsku-list.md). 

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.ReadWrite.All, Directory.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | User.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|addLicenses|[assignedLicense](../resources/assignedlicense.md)-Sammlung|Eine Auflistung von [AssignedLicense](../resources/assignedlicense.md) -Objekten, die die hinzuzufügenden Lizenzen angeben. Sie können eine Lizenz zugeordnet sind, indem die **DisabledPlans** -Eigenschaft für ein Objekt [AssignedLicense](../resources/assignedlicense.md) ServicePlans deaktivieren.|
|removeLicenses|Guid|Eine Auflistung von SkuIds, die die zu entfernenden Lizenzen zu identifizieren.|

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eine aktualisierte [Benutzer](../resources/user.md) -Objekt aus der Antwort.

## <a name="example"></a>Beispiel
Lizenzen für den Benutzer hinzufügen.
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```

## <a name="example"></a>Beispiel
Entfernen Sie Lizenzen vom Benutzer.

#####<a name="request"></a>Anforderung
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a>Antwort
In beiden Beispielen wird die Antwort das aktualisierte Benutzerobjekt. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
