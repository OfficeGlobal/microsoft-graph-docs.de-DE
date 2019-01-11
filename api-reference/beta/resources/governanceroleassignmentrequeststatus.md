---
title: Ressourcentyp governanceRoleAssignmentRequestStatus
description: Stellt den Status der GovernanceRoleAssignmentRequest dar.
localization_priority: Normal
ms.openlocfilehash: c5daac53661cc607d51e5bfd1ec9031cfa599fca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808071"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>Ressourcentyp governanceRoleAssignmentRequestStatus

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt den Status der [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)dar.


## <a name="properties"></a>Eigenschaften
Eigenschaft       | Typ |Beschreibung|
|:----|:-------------|:-----|
|status |Zeichenfolge| Der Status der Anforderung Zuordnung Rolle. Der Wert kann sein `InProgress` oder `Closed`.|
|Untergeordneter |Zeichenfolge| Der Sub Status der Anforderung Zuordnung Rolle. Die Werte sind möglich `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, und `ProvisioningStarted`.|
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
