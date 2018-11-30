---
title: Gemeinsame Liste
description: Berechnete Insight, der die Liste der Dateien, die ein Benutzer freigegeben zurückgibt.
ms.openlocfilehash: 589cb8da4ecb82149d11e0ad518d5a37749cc3da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065425"
---
# <a name="list-shared"></a>Gemeinsame Liste

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Berechnete Insight, der die Liste der Dateien, die ein Benutzer freigegeben zurückgibt.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
```http
GET /me/insights/shared
```
Fordern Sie mit einer 'Benutzer-Id"oder"UserPrincipalName"ist nur verfügbar, durch den Benutzer, die nicht von einer anderen Person:
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

Sie können die `$filter` Parameter zum Filtern von freigegebenen Elemente Abfragen. Beispielsweise basierend auf:

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

Finden Sie die verfügbaren Containertypen und Typen, die Sie nach [ResourceVisualization](../resources/insights-resourcevisualization.md)filtern können.

Sie können auch von einem bestimmten Benutzer gemeinsam genutzte Dateien abrufen. Beispielsweise durch Angabe der `lastshared/sharedby/address` Eigenschaft:

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

Finden Sie unter den komplexen Typ [SharingDetail](../resources/insights-sharingdetail.md) .


## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       |  Wert|
|:-------------|:------|
| Authorization  | Bearer {token}. Erforderlich.|
| Accept  | application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste der [freigegebenen](../resources/insights-shared.md) Elemente im Antworttext.
## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastShared" : { 
                "sharedDateTime" : "sharedDateTime-value",  
                "sharingSubject" : "sharingSubject-value",
                "sharingType" : "sharingType-value", 
                "sharedBy" : { 
                    "displayName" : "displayName-value", 
                    "id": "id-value" 
                }
                "sharingReference" : { 
                    "webUrl" : "webUrl-value",
                    "type: "type-value", 
                    "id": "id-value"
                } 
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
```

### <a name="expanding-resource"></a>Erweitern der Ressource
Die Ressource, die durch einen freigegebenen Einblick kann erweitert werden.
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```