---
title: Ressourcentyp governanceRoleAssignmentRequestStatus
description: Stellt den Status der GovernanceRoleAssignmentRequest dar.
ms.openlocfilehash: 06b0f17513d5d796d3fe71cbd3888963bc4a34ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059773"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>Ressourcentyp governanceRoleAssignmentRequestStatus

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->