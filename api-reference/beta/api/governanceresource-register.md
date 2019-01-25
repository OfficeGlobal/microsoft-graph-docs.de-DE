---
title: GovernanceResource registrieren
description: Registrieren Sie ein Objekt nicht verwalteten GovernanceResource in PIM.
localization_priority: Normal
ms.openlocfilehash: f65c8b5884f08377967d3418bade0d5fc70c2063
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519045"
---
# <a name="register-governanceresource"></a>GovernanceResource registrieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Registrieren Sie ein Objekt nicht verwalteten [GovernanceResource](../resources/governanceresource.md) in privilegierten Identity Management.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

>**Hinweis:** Diese API erfordert auch, dass die anfordernde Person mindestens eine aktive Rolle-Zuordnung für die Ressource verfügen.

|Berechtigungstyp      | Berechtigungen              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | PrivilegedAccess.ReadWrite.AzureResources  |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die **nur** die `$select` und `$expand` [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.

### <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|

### <a name="request-body"></a>Anforderungstext

|Parameter      |Typ                 |Erforderlich |Beschreibung|
|:-------------|:----------------------|:--------|:----------|
|externalId    |String                 |✓        |Die ExternalId der Ressource in PIM registriert werden.|

### <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwort.

### <a name="example"></a>Beispiel
In diesem Beispiel wird gezeigt, wie ein Azure-Abonnement Wingtip Toys - "Bemerkungen" registriert.
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a>Anforderung
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a>Antwort
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-register.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
