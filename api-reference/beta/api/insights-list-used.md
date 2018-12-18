---
title: Verwendet wird
description: Berechnete Insight, der die Liste der Dateien mit einem Benutzer zurückgibt.
author: simonhult
ms.openlocfilehash: 17f47e4e82d5cb038438b5d164c76371221de11a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342497"
---
# <a name="list-used"></a>Verwendet wird

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Berechnete Insight, der die Liste der Dateien mit einem Benutzer zurückgibt.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
```http
GET /me/insights/used
```
Anfordern eines anderen Benutzers verwendete Dokumente gibt Ergebnisse sortiert nach 'LastModifiedDateTime' und 'LastAccessedDateTime' auf 'LastModifiedDateTime' festgelegt ist.
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

Sie können die `$filter` Abfragen Parameter zum Filtern verwendet von Elementen. Beispielsweise basierend auf:

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

Basierend auf Containertyp oder:

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

Finden Sie die verfügbaren Containertypen und Typen, die Sie nach [ResourceVisualization](../resources/insights-resourcevisualization.md)filtern können.


## <a name="request-headers"></a>Anforderungsheader
| Header       |  Wert|
|:-------------|:------|
| Authorization  | Bearer {token}. Erforderlich.|
| Accept  | application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste der Elemente im Antworttext [verwendet](../resources/insights-used.md) .
## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben. 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
            }
        }
    ]
}
```

### <a name="expanding-resource"></a>Erweitern der Ressource
Die Ressource, die durch eine verwendeten Erkenntnisse kann erweitert werden.
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
