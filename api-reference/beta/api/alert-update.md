---
title: Warnung aktualisieren
description: Warnung Eigenschaft bearbeitbare in eine integrierte Lösung alert Status und Aufgaben in Lösungen synchron zu aktualisieren.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b1fec6bfca2ce116bc35c4a7c8a115418b15012
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967326"
---
# <a name="update-alert"></a>Warnung aktualisieren

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren einer bearbeitbaren **Benachrichtigung** -Eigenschaft in eine integrierte Lösung alert Status und Aufgaben in Lösungen synchron. Dieser Methode wird jede Lösung, die eine Aufzeichnung die Warnung ID wurde aktualisiert.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |   SecurityEvents.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht unterstützt  |
|Anwendung | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

> **Hinweis:** Sie müssen die **Warnung** -ID als Parameter und VendorInformation mit einschließen die `provider` und `vendor` mit dieser Methode.
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>Anforderungsheader

| Name       | Beschreibung|
|:-----------|:-----------|
| Authorization  | Bearer {code}. Erforderlich.|
|Prefer | zurückgeben = Darstellung |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Werte für die entsprechenden Felder, die aktualisiert werden soll. Der Textkörper **muss** enthalten die `vendorInformation` -Eigenschaft mit gültigen `provider` und `vendor` Felder. In der folgenden Tabelle werden die Felder, die für eine Warnung aktualisiert werden können. Die Werte für vorhandene Eigenschaften, die nicht im Textkörper Anforderung enthalten sind, werden nicht geändert. Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|assignedTo|Zeichenfolge|Name des der Analyst die Benachrichtigung wird für die Ursachenanalyse, Untersuchung oder Remediation zugewiesen.|
|closedDateTime|DateTimeOffset|Zeitpunkt, an dem die Benachrichtigung geschlossen wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|comments|String collection|Analystenkommentare auf die Benachrichtigung (für Kunden alert Management).|
|Feedback|AlertFeedback-Enumeration|Analyst Feedback auf die Benachrichtigung. Mögliche Werte: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|AlertStatus-Enumeration|Warnung Lebenszyklus-Status (Phase). Mögliche Werte: `unknown`, `newAlert`, `inProgress`, `resolved`.|
|tags|Zeichenfolgenauflistung|Benutzer definierbare Beschriftungen, die auf eine Warnung angewendet werden können und als filterbedingungen (beispielsweise "HVA", "MAUERN) dienen.|
|vendorInformation |[securityVendorInformation](../resources/securityvendorinformation.md)|Komplexer Typ, das Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider enthält (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker). **Anbieter und Hersteller Felder sind erforderlich.**|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode eine `200 OK` Antwortcode und das aktualisierte [Warnung](../resources/alert.md) -Objekt aus der Antwort.

## <a name="examples"></a>Beispiele

### <a name="example-1-request-without-prefer-header"></a>In Beispiel 1: Anforderung ohne bevorzugen-header

#### <a name="request"></a>Anforderung

Im folgenden ist ein Beispiel für die Anforderung ohne die `Prefer` Kopfzeile.
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Antwort

Es folgt ein Beispiel für eine erfolgreiche Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>Beispiel 2: Anforderung mit bevorzugen-header

#### <a name="request"></a>Anforderung

Das folgende Beispiel zeigt eine Anforderung, die umfasst die `Prefer` Anforderungsheader.

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

#### <a name="response"></a>Antwort

Im folgenden ist ein Beispiel für die Antwort bei der optionalen `Prefer: return=representation` Anforderungsheader wird verwendet.

>**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
