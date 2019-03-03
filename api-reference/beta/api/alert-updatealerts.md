---
title: 'Warnung: updateAlerts'
description: Aktualisieren Sie mehrere Warnungen in einer Anforderung anstelle mehrerer Anforderungen.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 5be6374d70baaf4205d5fc1e431111844ce34313
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366994"
---
# <a name="alert-updatealerts"></a>Warnung: updateAlerts

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie mehrere Warnungen in einer Anforderung anstelle mehrerer Anforderungen.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
|:---------------------------------------|:--------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |   SecurityEvents.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht unterstützt  |
|Anwendung | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a>Anforderungsheader

| Name          | Beschreibung   |
|:--------------|:--------------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an. Jede Entität muss über **ID** -und **vendorInformation** -Eigenschaften verfügen. Ausführliche Informationen zu Eigenschaften, die aktualisiert werden können, finden Sie unter [updatealert](alert-update.md).

| Parameter    | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|Wert|[Warnungs](../resources/alert.md) Sammlung| Sammlung von zu aktualisierende Warnungen. Jede Entität muss **ID**, **vendorInformation**und andere bearbeitbare Eigenschaften haben, die aktualisiert werden müssen.|

## <a name="response"></a>Antwort

Bei erfolgreicher Ausführung gibt diese Methode `200, OK` den Antwortcode und das [Alert](../resources/alert.md) -Auflistungsobjekt im Antworttext zurück.

## <a name="examples"></a>Beispiele

Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "alert_updatealerts"
}-->

```http
POST https://graph.microsoft.com/beta/security/alerts/updateAlerts
Content-type: application/json

{
  "value": [
    {
      "assignedTo": "String",
      "closedDateTime": "String (timestamp)",
      "comments": ["String"],
      "feedback": "@odata.type: microsoft.graph.alertFeedback",
      "id": "String (identifier)",
      "status": "@odata.type: microsoft.graph.alertStatus",
      "tags": ["String"],
      "vendorInformation":
        {
          "provider": "String",
          "vendor": "String"
        }
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
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert: updateAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
