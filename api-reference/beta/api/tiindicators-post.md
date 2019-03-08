---
title: Bedrohungs Intelligenz-Indikator erstellen
description: Erstellen Sie eine neue tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 440515a45b4c530f32dd20fe29497e338b54a6bf
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481440"
---
# <a name="create-threat-intelligence-indicator"></a>Bedrohungs Intelligenz-Indikator erstellen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Erstellen eines neuen [tiIndicator](../resources/tiindicator.md) -Objekts.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
|:---------------------------------------|:--------------------------------------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | ThreatIndicators.ReadWrite.OwnedBy  |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
| Anwendung                            | ThreatIndicators.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a>Anforderungsheader

| Name          | Beschreibung   |
|:--------------|:--------------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext eine JSON-Darstellung eines [tiIndicator](../resources/tiindicator.md) -Objekts an, das mindestens eine zu beobachtbare [e-Mail](../resources/tiindicator.md#indicator-observables---email), [Datei](../resources/tiindicator.md#indicator-observables---file)oder ein [Netzwerk](../resources/tiindicator.md#indicator-observables---network) enthält.

## <a name="response"></a>Antwort

Bei erfolgreicher Ausführung gibt diese Methode `201 Created` den Antwortcode und ein [tiIndicator](../resources/tiindicator.md) -Objekt im Antworttext zurück.

## <a name="examples"></a>Beispiele

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "create_tiindicator_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators
Content-type: application/json

{
  "action": "alert",
  "activityGroupNames": [],
  "confidence": 0,
  "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
  "expirationDateTime": "2019-03-01T21:43:37.5031462+00:00",
  "externalId": "Test--8586509942679764298MS501",
  "fileHashType": "sha256",
  "fileHashValue": "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313",
  "killChain": [],
  "malwareFamilyNames": [],
  "severity": 0,
  "tags": [],
  "targetProduct": "Azure Sentinel",
  "threatType": "WatchList",
  "tlpLevel": "green"
}
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

> [!NOTE]
> Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXX",
    "action": "alert",
    "additionalInformation": null,
    "activityGroupNames": [],
    "confidence": 0,
    "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
