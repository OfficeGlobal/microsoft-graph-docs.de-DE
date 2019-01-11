---
title: Ressourcentyp privilegedAccess
description: " beispielsweise `privilegedAccess/azureResources` PIM Verwalten von Azure Ressourcen Systemzugriff darstellt."
localization_priority: Normal
ms.openlocfilehash: f4166fb539d627730c68c7e039fd8d672ff4c785
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810052"
---
# <a name="privilegedaccess-resource-type"></a><span data-ttu-id="03a8b-103">Ressourcentyp privilegedAccess</span><span class="sxs-lookup"><span data-stu-id="03a8b-103">privilegedAccess resource type</span></span>

> <span data-ttu-id="03a8b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="03a8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03a8b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="03a8b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03a8b-106">Stellt eine Gruppe von Funktionen, die vom Dienst privilegierten Identity Management (PIM) bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="03a8b-106">Represents a group of functionalities provided by the Privileged Identity Management (PIM) service.</span></span> <span data-ttu-id="03a8b-107">Unterschiedliche Instanzen von `privilegedAccess` darstellen von anderen Anbietern von PIM; verwaltet werden beispielsweise `privilegedAccess/azureResources` PIM Verwalten von Azure Ressourcen Systemzugriff darstellt.</span><span class="sxs-lookup"><span data-stu-id="03a8b-107">Different instances of `privilegedAccess` represent different providers managed by PIM; for example, `privilegedAccess/azureResources` represents PIM managing privileged access to Azure resources.</span></span>


<span data-ttu-id="03a8b-108">`privilegedAccess`Jetzt ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="03a8b-108">`privilegedAccess` is read-only for now.</span></span> <span data-ttu-id="03a8b-109">Nicht `POST`, `PUT`, `PATCH`, oder `DELETE` Vorgänge werden unterstützt, auf die `privilegedAccess` Entität festlegen.</span><span class="sxs-lookup"><span data-stu-id="03a8b-109">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `privilegedAccess` entity set.</span></span>

## <a name="properties"></a><span data-ttu-id="03a8b-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="03a8b-110">Properties</span></span>
| <span data-ttu-id="03a8b-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03a8b-111">Property</span></span>  | <span data-ttu-id="03a8b-112">Typ</span><span class="sxs-lookup"><span data-stu-id="03a8b-112">Type</span></span>      |<span data-ttu-id="03a8b-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03a8b-113">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="03a8b-114">id</span><span class="sxs-lookup"><span data-stu-id="03a8b-114">id</span></span>         |<span data-ttu-id="03a8b-115">String</span><span class="sxs-lookup"><span data-stu-id="03a8b-115">String</span></span>     |<span data-ttu-id="03a8b-116">Die Id des Anbieters von PIM verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="03a8b-116">The id of the provider managed by PIM.</span></span>|
|<span data-ttu-id="03a8b-117">displayName</span><span class="sxs-lookup"><span data-stu-id="03a8b-117">displayName</span></span>|<span data-ttu-id="03a8b-118">String</span><span class="sxs-lookup"><span data-stu-id="03a8b-118">String</span></span>     |<span data-ttu-id="03a8b-119">Der Anzeigename des Anbieters von PIM verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="03a8b-119">The display name of the provider managed by PIM.</span></span>|


## <a name="relationships"></a><span data-ttu-id="03a8b-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="03a8b-120">Relationships</span></span>
| <span data-ttu-id="03a8b-121">Beziehung</span><span class="sxs-lookup"><span data-stu-id="03a8b-121">Relationship</span></span>   | <span data-ttu-id="03a8b-122">Typ</span><span class="sxs-lookup"><span data-stu-id="03a8b-122">Type</span></span>                                         |<span data-ttu-id="03a8b-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03a8b-123">Description</span></span>|
|:---------------|:---------------------------------------------|:----------|
|<span data-ttu-id="03a8b-124">resources</span><span class="sxs-lookup"><span data-stu-id="03a8b-124">resources</span></span>       |<span data-ttu-id="03a8b-125">[GovernanceResource](../resources/governanceresource.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="03a8b-125">[governanceResource](../resources/governanceresource.md) collection</span></span>            |<span data-ttu-id="03a8b-126">Eine Auflistung von Ressourcen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="03a8b-126">A collection of resources for the provider.</span></span>|
|<span data-ttu-id="03a8b-127">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="03a8b-127">roleAssignments</span></span> |<span data-ttu-id="03a8b-128">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="03a8b-128">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="03a8b-129">Eine Auflistung von rollenzuweisungen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="03a8b-129">A collection of role assignments for the provider.</span></span>|
|<span data-ttu-id="03a8b-130">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="03a8b-130">roleDefinitions</span></span> |<span data-ttu-id="03a8b-131">[GovernanceRoleDefinition](../resources/governanceroledefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="03a8b-131">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span>|<span data-ttu-id="03a8b-132">Eine Auflistung von Definitionen für den Anbieter Rolle.</span><span class="sxs-lookup"><span data-stu-id="03a8b-132">A collection of role defintions for the provider.</span></span>|
|<span data-ttu-id="03a8b-133">roleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="03a8b-133">roleAssignmentRequests</span></span> |<span data-ttu-id="03a8b-134">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="03a8b-134">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection</span></span>|<span data-ttu-id="03a8b-135">Eine Auflistung von Role Assignment-Anforderungen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="03a8b-135">A collection of role assignment requests for the provider.</span></span>|
|<span data-ttu-id="03a8b-136">roleSettings</span><span class="sxs-lookup"><span data-stu-id="03a8b-136">roleSettings</span></span> |<span data-ttu-id="03a8b-137">[GovernanceRoleSetting](../resources/governancerolesetting.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="03a8b-137">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="03a8b-138">Eine Auflistung von Einstellungen für Serverrollen für den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="03a8b-138">A collection of role settings for the provider.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="03a8b-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="03a8b-139">JSON representation</span></span>

<span data-ttu-id="03a8b-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="03a8b-140">Here is a JSON representation of the resource.</span></span>

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
