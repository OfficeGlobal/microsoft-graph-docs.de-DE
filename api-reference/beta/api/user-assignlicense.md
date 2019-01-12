---
title: assignLicense
description: Hinzufügen oder Entfernen von Lizenzen für den Benutzer aktivieren oder Deaktivieren der Verwendung von Microsoft-Cloud-angeboten. Beispielsweise eine Organisation kann ein Office 365 Enterprise E3-Abonnement mit 100 Lizenzen verfügen, und diese Anforderung weist eine der Lizenzen, die für einen bestimmten Benutzer. Sie können auch aktivieren und Deaktivieren von bestimmten Pläne ein Abonnement zugeordnet. Weitere Informationen zu Abonnements und Lizenzen finden Sie unter Technet-Artikel.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82347f46855baa91b5a42452cdbacc914bc89cdd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933792"
---
# <a name="assignlicense"></a>assignLicense

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
| Header       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|addLicenses|[assignedLicense](../resources/assignedlicense.md) collection|Eine Auflistung von [AssignedLicense](../resources/assignedlicense.md) -Objekten, die die hinzuzufügenden Lizenzen angeben. Sie können eine Lizenz zugeordnet sind, indem die **DisabledPlans** -Eigenschaft für ein Objekt [AssignedLicense](../resources/assignedlicense.md) ServicePlans deaktivieren.|
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
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
