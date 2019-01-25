---
title: Ressourcentyp governanceRoleAssignmentRequestStatus
description: Stellt den Status der GovernanceRoleAssignmentRequest dar.
localization_priority: Normal
ms.openlocfilehash: f4f0b23cf13de5beedb1964484ec4fbbb6e98720
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510176"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>Ressourcentyp governanceRoleAssignmentRequestStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt den Status der [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)dar.


## <a name="properties"></a>Eigenschaften
Eigenschaft       | Typ |Beschreibung|
|:----|:-------------|:-----|
|status |String| Der Status der Anforderung Zuordnung Rolle. Der Wert kann sein `InProgress` oder `Closed`.|
|Untergeordneter |String| Der Sub Status der Anforderung Zuordnung Rolle. Die Werte sind möglich `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, und `ProvisioningStarted`.|
|statusDetails       |[KeyValue](../resources/keyvalue.md) -Auflistung| Die Details des Status der Anforderung Zuordnung Rolle. Es stellt die Ergebnisse der Auswertung der verschiedenen Regeln. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyvalue"}],
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequeststatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
