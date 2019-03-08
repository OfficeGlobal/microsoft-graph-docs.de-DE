---
title: SecurityActions aufListen
description: Abrufen einer Liste von SecurityAction-Objekten.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1a161fd6113e6f29b061bd1dca9d2c4b16d7ee9c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482315"
---
# <a name="list-securityactions"></a>SecurityActions aufListen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abrufen einer Liste von [SecurityAction](../resources/securityaction.md) -Objekten.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
|:---------------------------------------|:--------------------------------------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | SecurityActions. Read. all, SecurityActions. ReadWrite. all |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
| Anwendung                            | SecurityActions. Read. all, SecurityActions. ReadWrite. all |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt einige der OData-Abfrageparameter zur Anpassung der Antwort. Allgemeine Informationen finden Sie unter [OData Query Parameters](/graph/query-parameters).

## <a name="request-headers"></a>Anforderungsheader

| Name      |Beschreibung|
|:----------|:----------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [SecurityAction](../resources/securityaction.md) -Objekten im Antworttext zurück.

## <a name="examples"></a>Beispiele

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_securityactions"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

> [!NOTE]
> Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "actionReason": "actionReason-value",
      "appId": "appId-value",
      "azureTenantId": "azureTenantId-value",
      "clientContext": "clientContext-value",
      "completedDateTime": "datetime-value",
      "createdDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List securityActions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
