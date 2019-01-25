---
title: Ressourcentyp privilegedApproval
description: Stellt eine Genehmigung, die für die erste in einer Rolle in privilegierten Identity Management angefordert wird.
localization_priority: Normal
ms.openlocfilehash: 283236d945e9a71a4ae0461bbefe66260efa88a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516889"
---
# <a name="privilegedapproval-resource-type"></a>Ressourcentyp privilegedApproval

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Genehmigung, die für die erste in einer Rolle in privilegierten Identity Management angefordert wird.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von privilegedApproval](../api/privilegedapproval-get.md) | [privilegedApproval](privilegedapproval.md) |Lesen Sie Eigenschaften und Beziehungen des PrivilegedApproval-Objekts.|
|[Objekte in der Liste privilegedApproval](../api/privilegedapproval-list.md) | [PrivilegedApproval](privilegedapproval.md) -Auflistung|Ruft die Auflistung der PrivilegedApproval.|
|[Erstellen von privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |PrivilegedApproval-Objekt zu erstellen. |
|[PrivilegedApproval aktualisieren](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |PrivilegedApproval-Objekt zu aktualisieren. |
|[Myrequests](../api/privilegedapproval-myrequests.md)|[privilegedApproval](privilegedapproval.md)|Get-Anforderungen für das jeweilige Genehmigung.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|approvalDuration|Dauer||
|approvalState|string| Mögliche Werte sind: `pending`, `approved`, `denied`, `aborted` und `canceled`.|
|approvalType|String||
|approverReason|String||
|endDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|id|String| Schreibgeschützt.|
|requestorReason|String||
|roleId|String||
|startDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|userId|String||

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Schreibgeschützt. Lässt Nullwerte zu.|
|Anforderung|[privilegedRoleAssignmentRequest](privilegedroleassignmentrequest.md)| Schreibgeschützt. Die Rolle Zuordnung Anforderung für dieses Objekt Genehmigung|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedapproval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
