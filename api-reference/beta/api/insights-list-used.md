---
title: Verwendet wird
description: Berechnete Insight, der die Liste der Dateien mit einem Benutzer zurückgibt.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: e73536d5933d6293539eb00ba8cdc2e85ce5fa93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526102"
---
# <a name="list-used"></a>Verwendet wird

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| Kopfzeile       |  Wert|
|:-------------|:------|
| Authorization  | Bearer {token}. Erforderlich.|
| Annehmen  | application/json|

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
