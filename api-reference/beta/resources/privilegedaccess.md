---
title: Ressourcentyp privilegedAccess
description: " beispielsweise `privilegedAccess/azureResources` PIM Verwalten von Azure Ressourcen Systemzugriff darstellt."
ms.openlocfilehash: af109c0cc355bfb282630d21cd02bb463b944f38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065769"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="82872-103">Ressourcentyp privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="82872-103">privilegedAccess resource type</span></span>

> <span data-ttu-id="82872-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="82872-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82872-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="82872-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82872-106">Stellt eine Gruppe von Funktionen, die vom Dienst privilegierten Identity Management (PIM) bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="82872-106">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="82872-107">Unterschiedliche Instanzen von `privilegedAccess` darstellen von anderen Anbietern von PIM; verwaltet werden beispielsweise `privilegedAccess/azureResources` PIM Verwalten von Azure Ressourcen Systemzugriff darstellt.</span><span class="sxs-lookup"><span data-stu-id="82872-107">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="82872-108">`privilegedAccess`Jetzt ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82872-108">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="82872-109">Nicht `POST`, `PUT`, `PATCH`, oder `DELETE` Vorgänge werden unterstützt, auf die `privilegedAccess` Entität festlegen.</span><span class="sxs-lookup"><span data-stu-id="82872-109">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="82872-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="82872-110">Properties</span></span>
| <span data-ttu-id="82872-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="82872-111">Property</span></span>  | <span data-ttu-id="82872-112">Typ</span><span class="sxs-lookup"><span data-stu-id="82872-112">Type</span></span>      |<span data-ttu-id="82872-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82872-113">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="82872-114">id</span><span class="sxs-lookup"><span data-stu-id="82872-114">id</span></span>         |<span data-ttu-id="82872-115">String</span><span class="sxs-lookup"><span data-stu-id="82872-115">String</span></span>     |<span data-ttu-id="82872-116">Die Id des Anbieters von PIM verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="82872-116">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="82872-117">displayName</span><span class="sxs-lookup"><span data-stu-id="82872-117">displayName</span></span>|<span data-ttu-id="82872-118">String</span><span class="sxs-lookup"><span data-stu-id="82872-118">String</span></span>     |<span data-ttu-id="82872-119">Der Anzeigename des Anbieters von PIM verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="82872-119">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="82872-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="82872-120">Relationships</span></span>
| <span data-ttu-id="82872-121">Beziehung</span><span class="sxs-lookup"><span data-stu-id="82872-121">Relationship</span></span>   | <span data-ttu-id="82872-122">Typ</span><span class="sxs-lookup"><span data-stu-id="82872-122">Type</span></span>                                         |<span data-ttu-id="82872-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82872-123">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="82872-124">resources</span><span class="sxs-lookup"><span data-stu-id="82872-124">resources</span></span>       |<span data-ttu-id="82872-125">[GovernanceResource](../resources/governanceresource.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="82872-125">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="82872-126">Eine Auflistung von Ressourcen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="82872-126">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="82872-127">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="82872-127">roleAssignments</span></span> |<span data-ttu-id="82872-128">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="82872-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="82872-129">Eine Auflistung von rollenzuweisungen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="82872-129">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="82872-130">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="82872-130">roleDefinitions</span></span> |<span data-ttu-id="82872-131">[GovernanceRoleDefinition](../resources/governanceroledefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="82872-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="82872-132">Eine Auflistung von Definitionen für den Anbieter Rolle.</span><span class="sxs-lookup"><span data-stu-id="82872-132">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="82872-133">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="82872-133">roleAssignmentRequests</span></span> |<span data-ttu-id="82872-134">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="82872-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="82872-135">Eine Auflistung von Role Assignment-Anforderungen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="82872-135">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="82872-136">roleSettings</span><span class="sxs-lookup"><span data-stu-id="82872-136">roleSettings</span></span> |<span data-ttu-id="82872-137">[GovernanceRoleSetting](../resources/governancerolesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="82872-137">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="82872-138">Eine Auflistung von Einstellungen für Serverrollen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="82872-138">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="82872-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="82872-139">JSON representation</span></span>

<span data-ttu-id="82872-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="82872-140">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
