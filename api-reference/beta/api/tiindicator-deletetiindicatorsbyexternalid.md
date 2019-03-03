---
title: 'tiIndicator: deleteTiIndicatorsByExternalId'
description: Löschen Sie mehrere Threat Intelligence (TI)-Indikatoren in einer Anforderung anstelle mehrerer Anforderungen, und die Anforderung enthält Externe IDs anstelle von IDs.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 82cdd0d9688e778982244a06a2a2e5d558d25807
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366945"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a>tiIndicator: deleteTiIndicatorsByExternalId

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Löschen Sie mehrere Threat Intelligence (TI)-Indikatoren in einer Anforderung anstelle mehrerer Anforderungen, wenn die Anforderung externe IDs anstelle von IDs enthält.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp  | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
|:---------------------------------------|:--------------------------------------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | ThreatIndicators. ReadWrite. OwnedBy |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
| Anwendung                            | ThreatIndicators. ReadWrite. OwnedBy |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a>Anforderungsheader

| Name          | Beschreibung   |
|:--------------|:--------------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|Wert|String collection| Auflistung der zu löschenden TiIndicator-Objekte. **** `externalIds` |

## <a name="response"></a>Antwort

Bei erfolgreicher Ausführung gibt diese Methode `200 OK` den Antwortcode und ein [resultInfo](../resources/resultinfo.md) -Auflistungsobjekt im Antworttext zurück.

## <a name="examples"></a>Beispiele

Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicatorsbyexternalid"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId
Content-type: application/json

{
  "value": [
    "externalId-value1",
    "externalId-value2"
  ]
}
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

> [!NOTE]
> Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "value": [
    {
      "code": "code-value",
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
