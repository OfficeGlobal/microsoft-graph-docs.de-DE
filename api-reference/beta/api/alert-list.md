---
title: Warnungen auflisten
description: Abrufen einer Liste der alert-Objekten.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d50c3244ae2c0e9f158dc38923136ef3e8656f0d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524380"
---
# <a name="list-alerts"></a>Warnungen auflisten

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abrufen einer Liste von [Warnung](../resources/alert.md) -Objekten.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  SecurityEvents.Read.All SecurityEvents.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht unterstützt  |
|Anwendung | SecurityEvents.Read.All SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die folgende [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top`Gibt die aggregierten Top-Ergebnisse aus jeder API Sicherheitsanbieter zurück.

Um eine alternative Eigenschaftensatz zurückzugeben, verwenden Sie die OData `$select` Abfragen Parameter, um die Gruppe von Eigenschaften der **Benachrichtigung** an, Sie werden soll.  Wenn **AssignedTo**, **Kategorie**und **Schweregrad** Eigenschaften zurückgeben möchten, fügen Sie beispielsweise die folgenden für Ihre Abfrage: `$select=assignedTo,category,severity`.

> **Hinweis:** `$top` darf maximal 1000 Warnungen und eine Kombination von `$top`  +  `$skip` 6000 Benachrichtigungen nicht überschreiten. Beispielsweise `/security/alerts?$top=10&$skip=5990` zurückgegebenen eine `200 OK` Antwortcode, aber `/security/alerts?$top=10&$skip=5991` zurückgegebenen eine `400 Bad Request` Antwortcode.  Weitere Informationen finden Sie unter [Microsoft Graph Security-API-Fehlerantworten](../resources/security-error-codes.md).

## <a name="request-headers"></a>Anforderungsheader

| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {code}. Erforderlich.|

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an. Textkörper der Anforderung wird ignoriert.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext **Benachrichtigung** . Wenn ein Statuscode als 2xx oder 404 von einem Anbieter zurückgegeben wird, oder wenn von ein Anbieter Zeitlimit überschritten, die Antwort werden eine `206 Partial Content` Statuscode mit der Anbieter Antwort in der Kopfzeile einer Warnung. Weitere Informationen finden Sie unter [Microsoft Graph Security-API-Fehlerantworten](../resources/security-error-codes.md).

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
