---
title: AufListen von Bedrohungs Ermittlungs Indikatoren
description: Ruft eine Liste von tiindicator-Objekten ab.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 98f058d94c101a2f664f21ea05252a51476b426d
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366910"
---
# <a name="list-threat-intelligence-indicators"></a>AufListen von Bedrohungs Ermittlungs Indikatoren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ruft eine Liste von [tiIndicator](../resources/tiindicator.md) -Objekten ab.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp     | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
|:---------------------------------------|:--------------------------------------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | ThreatIndicators. ReadWrite. OwnedBy  |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
| Anwendung                            | ThreatIndicators. ReadWrite. OwnedBy |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators
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

Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [tiIndicator](../resources/tiindicator.md) -Objekten im Antworttext zurück.

## <a name="examples"></a>Beispiele

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_tiindicators"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

> [!NOTE]
> Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "action": "action-value",
      "activityGroupNames": [
        "activityGroupNames-value"
      ],
      "additionalInformation": "additionalInformation-value",
      "azureTenantId": "azureTenantId-value",
      "confidence": 99,
      "description": "description-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
