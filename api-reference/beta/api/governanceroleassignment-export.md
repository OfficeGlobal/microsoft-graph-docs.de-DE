---
title: Exportieren von governanceRoleAssignmentRequests
description: Abrufen einer Auflistung von GovernanceRoleAssignmentRequests im Format `application/octet-stream`, die als CSV-Datei im Browser analysiert werden können.
localization_priority: Normal
ms.openlocfilehash: 10fd7c720bf7b6f162a4d8c2189e81a9205e53ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828728"
---
# <a name="export-governanceroleassignmentrequests"></a>Exportieren von governanceRoleAssignmentRequests

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Abrufen einer Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) im Format `application/octet-stream`, die als CSV-Datei im Browser analysiert werden können.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | PrivilegedAccess.ReadWrite.AzureResources  |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | PrivilegedAccess.ReadWrite.AzureResources |


## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->Exportieren Sie eine Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) für eine Ressource
    
>**Hinweis:** Neben den Berechtigungsbereich erfordert dieser Anforderung den Requestor, mindestens eine rollenzuweisung auf die Ressource verfügbar ist. 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

Exportieren Sie eine Auflistung von [GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) davon.
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.

## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Inhalte vom Typ `application/octet-stream`.

## <a name="example"></a>Beispiel
In diesem Beispiel werden alle rollenzuweisungen als CSV-Datei in das Abonnement Wingtip Toys - "Bemerkungen" gespeichert. 

##### <a name="request"></a>Anforderung
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
