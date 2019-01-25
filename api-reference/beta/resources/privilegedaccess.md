---
title: Ressourcentyp privilegedAccess
description: " beispielsweise `privilegedAccess/azureResources` PIM Verwalten von Azure Ressourcen Systemzugriff darstellt."
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512927"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="65abe-103">Ressourcentyp privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="65abe-103">privilegedAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65abe-104">Stellt eine Gruppe von Funktionen, die vom Dienst privilegierten Identity Management (PIM) bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="65abe-104">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="65abe-105">Unterschiedliche Instanzen von `privilegedAccess` darstellen von anderen Anbietern von PIM; verwaltet werden beispielsweise `privilegedAccess/azureResources` PIM Verwalten von Azure Ressourcen Systemzugriff darstellt.</span><span class="sxs-lookup"><span data-stu-id="65abe-105">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="65abe-106">`privilegedAccess`Jetzt ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="65abe-106">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="65abe-107">Nicht `POST`, `PUT`, `PATCH`, oder `DELETE` Vorgänge werden unterstützt, auf die `privilegedAccess` Entität festlegen.</span><span class="sxs-lookup"><span data-stu-id="65abe-107">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="65abe-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="65abe-108">Properties</span></span>
| <span data-ttu-id="65abe-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65abe-109">Property</span></span>  | <span data-ttu-id="65abe-110">Typ</span><span class="sxs-lookup"><span data-stu-id="65abe-110">Type</span></span>      |<span data-ttu-id="65abe-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65abe-111">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="65abe-112">id</span><span class="sxs-lookup"><span data-stu-id="65abe-112">id</span></span>         |<span data-ttu-id="65abe-113">String</span><span class="sxs-lookup"><span data-stu-id="65abe-113">String</span></span>     |<span data-ttu-id="65abe-114">Die Id des Anbieters von PIM verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="65abe-114">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="65abe-115">displayName</span><span class="sxs-lookup"><span data-stu-id="65abe-115">displayName</span></span>|<span data-ttu-id="65abe-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65abe-116">String</span></span>     |<span data-ttu-id="65abe-117">Der Anzeigename des Anbieters von PIM verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="65abe-117">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="65abe-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="65abe-118">Relationships</span></span>
| <span data-ttu-id="65abe-119">Beziehung</span><span class="sxs-lookup"><span data-stu-id="65abe-119">Relationship</span></span>   | <span data-ttu-id="65abe-120">Typ</span><span class="sxs-lookup"><span data-stu-id="65abe-120">Type</span></span>                                         |<span data-ttu-id="65abe-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65abe-121">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="65abe-122">resources</span><span class="sxs-lookup"><span data-stu-id="65abe-122">resources</span></span>       |<span data-ttu-id="65abe-123">[GovernanceResource](../resources/governanceresource.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="65abe-123">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="65abe-124">Eine Auflistung von Ressourcen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="65abe-124">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="65abe-125">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="65abe-125">roleAssignments</span></span> |<span data-ttu-id="65abe-126">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="65abe-126">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="65abe-127">Eine Auflistung von rollenzuweisungen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="65abe-127">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="65abe-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="65abe-128">roleDefinitions</span></span> |<span data-ttu-id="65abe-129">[GovernanceRoleDefinition](../resources/governanceroledefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="65abe-129">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="65abe-130">Eine Auflistung von Definitionen für den Anbieter Rolle.</span><span class="sxs-lookup"><span data-stu-id="65abe-130">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="65abe-131">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="65abe-131">roleAssignmentRequests</span></span> |<span data-ttu-id="65abe-132">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="65abe-132">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="65abe-133">Eine Auflistung von Role Assignment-Anforderungen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="65abe-133">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="65abe-134">roleSettings</span><span class="sxs-lookup"><span data-stu-id="65abe-134">roleSettings</span></span> |<span data-ttu-id="65abe-135">[GovernanceRoleSetting](../resources/governancerolesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="65abe-135">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="65abe-136">Eine Auflistung von Einstellungen für Serverrollen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="65abe-136">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="65abe-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="65abe-137">JSON representation</span></span>

<span data-ttu-id="65abe-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="65abe-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
