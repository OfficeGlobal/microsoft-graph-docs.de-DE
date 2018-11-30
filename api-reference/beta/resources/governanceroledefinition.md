---
title: Ressourcentyp governanceRoleDefinition
description: Stellt die Rollendefinitionen. Für Azure Ressourcen können sie Azure RBAC-Rollen, wie Besitzer, Leser, Autor darstellen.
ms.openlocfilehash: 057d74276b41abad47eb60ce48a99f1160c401ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059779"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="91f4b-104">Ressourcentyp governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="91f4b-104">governanceRoleDefinition resource type</span></span>

> <span data-ttu-id="91f4b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91f4b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91f4b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91f4b-106">Use of these APIs in production applications is not supported.</span></span> 


<span data-ttu-id="91f4b-107">Stellt die Rollendefinitionen.</span><span class="sxs-lookup"><span data-stu-id="91f4b-107">Represents the role definitions.</span></span> <span data-ttu-id="91f4b-108">Für Azure Ressourcen können sie Azure RBAC-Rollen, wie Besitzer, Leser, Autor darstellen.</span><span class="sxs-lookup"><span data-stu-id="91f4b-108">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="91f4b-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="91f4b-109">Methods</span></span>

| <span data-ttu-id="91f4b-110">Methode</span><span class="sxs-lookup"><span data-stu-id="91f4b-110">Method</span></span>          | <span data-ttu-id="91f4b-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="91f4b-111">Return Type</span></span> |<span data-ttu-id="91f4b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91f4b-112">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="91f4b-113">List</span><span class="sxs-lookup"><span data-stu-id="91f4b-113">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="91f4b-114">[GovernanceRoleDefinition](../resources/governanceroledefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="91f4b-114">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="91f4b-115">Eine Auflistung von Rollendefinitionen für eine Ressource aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="91f4b-115">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="91f4b-116">Get</span><span class="sxs-lookup"><span data-stu-id="91f4b-116">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="91f4b-117">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="91f4b-117">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="91f4b-118">Lesen Sie Eigenschaften und Beziehungen einer Rolle Definition Entität nach Id angegeben.</span><span class="sxs-lookup"><span data-stu-id="91f4b-118">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="91f4b-119">Nicht `POST`, `PUT`, `PATCH`, `DELETE` wird auf unterstützt `roleDefinitions` Entität-Set für jetzt.</span><span class="sxs-lookup"><span data-stu-id="91f4b-119">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="91f4b-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91f4b-120">Properties</span></span>
| <span data-ttu-id="91f4b-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91f4b-121">Property</span></span>  | <span data-ttu-id="91f4b-122">Typ</span><span class="sxs-lookup"><span data-stu-id="91f4b-122">Type</span></span>      |<span data-ttu-id="91f4b-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91f4b-123">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="91f4b-124">id</span><span class="sxs-lookup"><span data-stu-id="91f4b-124">id</span></span>         |<span data-ttu-id="91f4b-125">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-125">String</span></span>     |<span data-ttu-id="91f4b-126">Die Id der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="91f4b-126">The id of the role definition.</span></span> |
|<span data-ttu-id="91f4b-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="91f4b-127">resourceId</span></span> |<span data-ttu-id="91f4b-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91f4b-128">String</span></span>     |<span data-ttu-id="91f4b-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="91f4b-129">Required.</span></span> <span data-ttu-id="91f4b-130">Die Id der Rollendefinition zugeordneten Ressource.</span><span class="sxs-lookup"><span data-stu-id="91f4b-130">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="91f4b-131">externalId</span><span class="sxs-lookup"><span data-stu-id="91f4b-131">externalId</span></span>   |<span data-ttu-id="91f4b-132">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-132">String</span></span>     |<span data-ttu-id="91f4b-133">Die externe Id der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="91f4b-133">The external id of the role definition.</span></span>|
|<span data-ttu-id="91f4b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="91f4b-134">displayName</span></span>|<span data-ttu-id="91f4b-135">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-135">String</span></span>     |<span data-ttu-id="91f4b-136">Der Anzeigename der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="91f4b-136">The display name of the role definition.</span></span>|
|<span data-ttu-id="91f4b-137">subjectCount</span><span class="sxs-lookup"><span data-stu-id="91f4b-137">subjectCount</span></span>|<span data-ttu-id="91f4b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="91f4b-138">Int32</span></span>     |<span data-ttu-id="91f4b-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="91f4b-139">Optional.</span></span> <span data-ttu-id="91f4b-140">Die Anzahl der Themen, die die Rolle zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="91f4b-140">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="91f4b-141">Es stellt den Status des Antragstellers Zugriff auf die Ressource.</span><span class="sxs-lookup"><span data-stu-id="91f4b-141">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="91f4b-142">Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=subjectCount` in der Abfrage.</span><span class="sxs-lookup"><span data-stu-id="91f4b-142">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="91f4b-143">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="91f4b-143">eligibleAssignmentCount</span></span>|<span data-ttu-id="91f4b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="91f4b-144">Int32</span></span>|<span data-ttu-id="91f4b-145">Optional.</span><span class="sxs-lookup"><span data-stu-id="91f4b-145">Optional.</span></span> <span data-ttu-id="91f4b-146">Die Anzahl von zu auswählbaren rollenzuweisungen Rollendefinition zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="91f4b-146">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="91f4b-147">Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=eligibleAssignmentCount` in der Abfrage.</span><span class="sxs-lookup"><span data-stu-id="91f4b-147">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="91f4b-148">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="91f4b-148">activeAssignmentCount</span></span>|<span data-ttu-id="91f4b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="91f4b-149">Int32</span></span>    |<span data-ttu-id="91f4b-150">Optional.</span><span class="sxs-lookup"><span data-stu-id="91f4b-150">Optional.</span></span> <span data-ttu-id="91f4b-151">Die Anzahl der aktiven rollenzuweisungen Rollendefinition zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="91f4b-151">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="91f4b-152">Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=activeAssignmentCount` in der Abfrage.</span><span class="sxs-lookup"><span data-stu-id="91f4b-152">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="91f4b-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="91f4b-153">Relationships</span></span>
| <span data-ttu-id="91f4b-154">Beziehung</span><span class="sxs-lookup"><span data-stu-id="91f4b-154">Relationship</span></span> | <span data-ttu-id="91f4b-155">Typ</span><span class="sxs-lookup"><span data-stu-id="91f4b-155">Type</span></span>   |<span data-ttu-id="91f4b-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91f4b-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91f4b-157">resource</span><span class="sxs-lookup"><span data-stu-id="91f4b-157">resource</span></span>|[<span data-ttu-id="91f4b-158">governanceResource</span><span class="sxs-lookup"><span data-stu-id="91f4b-158">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="91f4b-159">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="91f4b-159">Read-only.</span></span> <span data-ttu-id="91f4b-160">Die zugeordneten Ressource für die Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="91f4b-160">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="91f4b-161">roleSetting</span><span class="sxs-lookup"><span data-stu-id="91f4b-161">roleSetting</span></span>|[<span data-ttu-id="91f4b-162">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="91f4b-162">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="91f4b-163">Die Einstellung der zugehörige Rolle für die Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="91f4b-163">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91f4b-164">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91f4b-164">JSON representation</span></span>

<span data-ttu-id="91f4b-165">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91f4b-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->