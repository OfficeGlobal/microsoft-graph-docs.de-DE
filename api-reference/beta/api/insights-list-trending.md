---
title: Liste Trend
description: Berechnete Insight, der die Liste der Elemente, um den Benutzer Trend zurückgibt.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 86b9daf96529d50d8767f234c3b1a6d9526eaac4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854789"
---
# <a name="list-trending"></a>Liste Trend

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Berechnete Insight, der die Liste der Elemente, um den Benutzer Trend zurückgibt.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

Sie können die `$filter` Parameter zum Filtern von Trend Elemente Abfragen. Beispielsweise basierend auf:

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

Basierend auf Containertyp oder:

`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

Finden Sie die verfügbaren Containertypen und Typen, die Sie nach [ResourceVisualization](../resources/insights-resourcevisualization.md)filtern können.


## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       |  Wert|
|:-------------|:------|
| Authorization  | Bearer {token}. Erforderlich.|
| Annehmen  | application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste der Elemente im Antworttext [Trend](../resources/insights-trending.md) . Jedes Element enthält Visualisierungseigenschaften für das Element in Ihre Erfahrung anzuzeigen.

## <a name="example"></a>Beispiel
#### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
```http
GET https://graph.microsoft.com/beta/me/insights/trending
```
#### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben. Finden Sie eine Beispiel ohne abgeschnittene Antwort am unteren Rand der Seite.
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```

### <a name="expanding-resource"></a>Erweitern der Ressource
Die Ressource, die durch einen Trend Einblick kann erweitert werden.
```http
GET https://graph.microsoft.com/beta/me/insights/trending/{id}/resource
```
