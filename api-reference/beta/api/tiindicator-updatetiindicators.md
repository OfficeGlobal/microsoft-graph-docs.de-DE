---
title: 'tiIndicator: updateTiIndicators'
description: Aktualisieren Sie mehrere Threat Intelligence-Indikatoren (TI) in einer Anforderung anstelle mehrerer Anforderungen.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 91020b533b621c1ba77b2f839d4e6ffd8d7ee8ac
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30367141"
---
# <a name="tiindicator-updatetiindicators"></a>tiIndicator: updateTiIndicators

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie mehrere Threat Intelligence-Indikatoren (TI) in einer Anforderung anstelle mehrerer Anforderungen.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp   | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
|:---------------------------------------|:--------------------------------------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | ThreatIndicators. ReadWrite. OwnedBy |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
| Anwendung                            | ThreatIndicators. ReadWrite. OwnedBy |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a>Anforderungsheader

| Name          | Beschreibung   |
|:--------------|:--------------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an. Ausführliche Informationen zu Eigenschaften, die aktualisiert werden können, finden Sie unter [Update tiIndicator](tiindicator-update.md).

| Parameter    | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|Wert|tiIndicator-Sammlung| Sammlung von **tiIndicators** , die aktualisiert werden soll. Jede Entität muss **ID** und andere bearbeitbare Eigenschaften haben, die aktualisiert werden müssen.|

## <a name="response"></a>Antwort

Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [tiIndicator](../resources/tiindicator.md) -Objekten im Antworttext zurück.

## <a name="examples"></a>Beispiele

Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "tiindicator_updatetiindicators"
}-->
```http
POST https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators
Content-type: application/json

{
  "value": [
    {
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "additionalInformation": "mytest"
    },
    {
      "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
      "additionalInformation": "test again"
    }
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
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "azureTenantId": "XXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": "mytest",
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a test indicator for demo purpose. Take no action on any observables set in this indicator.",
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: updateTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
