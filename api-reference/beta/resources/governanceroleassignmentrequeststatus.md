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
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="744d4-103">Ressourcentyp governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="744d4-103">governanceRoleAssignmentRequestStatus resource type</span></span>

> <span data-ttu-id="744d4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="744d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="744d4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="744d4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="744d4-106">Stellt den Status der [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)dar.</span><span class="sxs-lookup"><span data-stu-id="744d4-106">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="744d4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="744d4-107">Properties</span></span>
<span data-ttu-id="744d4-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="744d4-108">Property</span></span>       | <span data-ttu-id="744d4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="744d4-109">Type</span></span> |<span data-ttu-id="744d4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="744d4-110">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="744d4-111">status</span><span class="sxs-lookup"><span data-stu-id="744d4-111">status</span></span> |<span data-ttu-id="744d4-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="744d4-112">String</span></span>| <span data-ttu-id="744d4-113">Der Status der Anforderung Zuordnung Rolle.</span><span class="sxs-lookup"><span data-stu-id="744d4-113">The status of the role assignment request.</span></span> <span data-ttu-id="744d4-114">Der Wert kann sein `InProgress` oder `Closed`.</span><span class="sxs-lookup"><span data-stu-id="744d4-114">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="744d4-115">Untergeordneter</span><span class="sxs-lookup"><span data-stu-id="744d4-115">subStatus</span></span> |<span data-ttu-id="744d4-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="744d4-116">String</span></span>| <span data-ttu-id="744d4-117">Der Sub Status der Anforderung Zuordnung Rolle.</span><span class="sxs-lookup"><span data-stu-id="744d4-117">The sub status of the role assignment request.</span></span> <span data-ttu-id="744d4-118">Die Werte sind möglich `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, und `ProvisioningStarted`.</span><span class="sxs-lookup"><span data-stu-id="744d4-118">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="744d4-119">statusDetails</span><span class="sxs-lookup"><span data-stu-id="744d4-119">statusDetails</span></span>       |<span data-ttu-id="744d4-120">[KeyValue](../resources/keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="744d4-120">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="744d4-121">Die Details des Status der Anforderung Zuordnung Rolle.</span><span class="sxs-lookup"><span data-stu-id="744d4-121">The details of the status of the role assignment request.</span></span> <span data-ttu-id="744d4-122">Es stellt die Ergebnisse der Auswertung der verschiedenen Regeln.</span><span class="sxs-lookup"><span data-stu-id="744d4-122">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="744d4-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="744d4-123">JSON representation</span></span>

<span data-ttu-id="744d4-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="744d4-124">Here is a JSON representation of the resource.</span></span>

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
