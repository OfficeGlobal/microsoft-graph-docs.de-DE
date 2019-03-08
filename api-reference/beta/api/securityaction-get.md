---
title: Get securityAction
description: Abrufen der Eigenschaften und Beziehungen des SecurityAction-Objekts.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 7bcad2d3249b0ac7c5bd08d3d61742e7dc5166d6
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482252"
---
# <a name="get-securityaction"></a>Get securityAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ruft die Eigenschaften und Beziehungen eines [SecurityAction](../resources/securityaction.md) -Objekts ab.

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
GET /security/securityActions/{id}
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

Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [SecurityAction](../resources/securityaction.md) -Objekt im Antworttext zurück.

## <a name="examples"></a>Beispiele

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

> [!NOTE]
> Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "actionReason": "actionReason-value",
  "appId": "appId-value",
  "azureTenantId": "azureTenantId-value",
  "clientContext": "clientContext-value",
  "completedDateTime": "datetime-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
