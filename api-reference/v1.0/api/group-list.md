---
title: Gruppen auflisten
description: Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5081c5013c1bf7c1a1bfbcff58afe5a83aa67bc9
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726575"
---
# <a name="list-groups"></a>Gruppen auflisten
Dient zum Auflisten aller in einer Organisation verfügbaren Gruppen, einschließlich, aber nicht beschränkt auf Office 365-Gruppen.

Dieser Vorgang gibt standardmäßig nur eine Untergruppe der Eigenschaften für jede Gruppe zurück. Diese Standardeigenschaften werden im Abschnitt [Eigenschaften](../resources/group.md#properties) aufgeführt. 

Um Eigenschaften abzurufen, die _nicht_ standardmäßig zurückgegeben werden, führen Sie eine [GET](group-get.md)-Operation für die Gruppe aus, und geben Sie die Eigenschaften in einer OData-Abfrageoption `$select` an. Sehen Sie sich das [Beispiel](group-get.md#request-2) an.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.Read.All, Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Um nur Office 365-Gruppen (auch als einheitliche Gruppen bezeichnet) aufzulisten, wenden Sie einen Filter auf **groupTypes** an: <!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

Sie können die OData-Abfrageoption `$orderby` verwenden, um Gruppen in einer Organisation nach ihrem jeweiligen Wert für **displayName** zu sortieren. Hier ein Beispiel: <!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

Weitere Informationen zu OData-Abfrageoptionen finden Sie unter [OData-Abfrageparameter](/graph/query-parameters).

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [group](../resources/group.md)-Objekten im Antworttext zurückgegeben. Die Antwort enthält nur die Standardeigenschaften der einzelnen Gruppen.

## <a name="example"></a>Beispiel
#### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.

>**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Alle Standardeigenschaften werden für jede Gruppe einem tatsächlichen Aufruf zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-12-22T02:21:05Z",
            "creationOptions": [],
            "description": "Self help community for golf",
            "displayName": "Golf Assist",
            "groupTypes": [
                "Unified"
            ],
            "mail": "golfassist@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golfassist",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golfassist@contoso.onmicrosoft.com",
                "SMTP:golfassist@contoso.com"
            ],
            "renewedDateTime": "2018-12-22T02:21:05Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": "Public",
            "onPremisesProvisioningErrors": []
        },
        {
            "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-11-19T20:29:40Z",
            "creationOptions": [],
            "description": "Talk about golf",
            "displayName": "Golf Discussion",
            "groupTypes": [],
            "mail": "golftalk@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golftalk",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golftalk@contoso.onmicrosoft.com",
                "SMTP:golftalk@contoso.com"
            ],
            "renewedDateTime": "2018-11-19T20:29:40Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": null,
            "onPremisesProvisioningErrors": []
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
