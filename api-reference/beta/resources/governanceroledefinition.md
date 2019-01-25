---
title: Ressourcentyp governanceRoleDefinition
description: Stellt die Rollendefinitionen. Für Azure Ressourcen können sie Azure RBAC-Rollen, wie Besitzer, Leser, Autor darstellen.
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528641"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="6ea1c-104">Ressourcentyp governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6ea1c-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="6ea1c-105">Stellt die Rollendefinitionen.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-105">Represents the role definitions.</span></span> <span data-ttu-id="6ea1c-106">Für Azure Ressourcen können sie Azure RBAC-Rollen, wie Besitzer, Leser, Autor darstellen.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="6ea1c-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="6ea1c-107">Methods</span></span>

| <span data-ttu-id="6ea1c-108">Methode</span><span class="sxs-lookup"><span data-stu-id="6ea1c-108">Method</span></span>          | <span data-ttu-id="6ea1c-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6ea1c-109">Return Type</span></span> |<span data-ttu-id="6ea1c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ea1c-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="6ea1c-111">List</span><span class="sxs-lookup"><span data-stu-id="6ea1c-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="6ea1c-112">[GovernanceRoleDefinition](../resources/governanceroledefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6ea1c-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="6ea1c-113">Eine Auflistung von Rollendefinitionen für eine Ressource aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="6ea1c-114">Get</span><span class="sxs-lookup"><span data-stu-id="6ea1c-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="6ea1c-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6ea1c-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="6ea1c-116">Lesen Sie Eigenschaften und Beziehungen einer Rolle Definition Entität nach Id angegeben.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="6ea1c-117">Nicht `POST`, `PUT`, `PATCH`, `DELETE` wird auf unterstützt `roleDefinitions` Entität-Set für jetzt.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="6ea1c-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ea1c-118">Properties</span></span>
| <span data-ttu-id="6ea1c-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ea1c-119">Property</span></span>  | <span data-ttu-id="6ea1c-120">Typ</span><span class="sxs-lookup"><span data-stu-id="6ea1c-120">Type</span></span>      |<span data-ttu-id="6ea1c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ea1c-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="6ea1c-122">id</span><span class="sxs-lookup"><span data-stu-id="6ea1c-122">id</span></span>         |<span data-ttu-id="6ea1c-123">string</span><span class="sxs-lookup"><span data-stu-id="6ea1c-123">String</span></span>     |<span data-ttu-id="6ea1c-124">Die Id der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-124">The id of the role definition.</span></span> |
|<span data-ttu-id="6ea1c-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="6ea1c-125">resourceId</span></span> |<span data-ttu-id="6ea1c-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ea1c-126">String</span></span>     |<span data-ttu-id="6ea1c-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-127">Required.</span></span> <span data-ttu-id="6ea1c-128">Die Id der Rollendefinition zugeordneten Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="6ea1c-129">externalId</span><span class="sxs-lookup"><span data-stu-id="6ea1c-129">externalId</span></span>   |<span data-ttu-id="6ea1c-130">String</span><span class="sxs-lookup"><span data-stu-id="6ea1c-130">String</span></span>     |<span data-ttu-id="6ea1c-131">Die externe Id der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="6ea1c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6ea1c-132">displayName</span></span>|<span data-ttu-id="6ea1c-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ea1c-133">String</span></span>     |<span data-ttu-id="6ea1c-134">Der Anzeigename der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="6ea1c-135">subjectCount</span><span class="sxs-lookup"><span data-stu-id="6ea1c-135">subjectCount</span></span>|<span data-ttu-id="6ea1c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea1c-136">Int32</span></span>     |<span data-ttu-id="6ea1c-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-137">Optional.</span></span> <span data-ttu-id="6ea1c-138">Die Anzahl der Themen, die die Rolle zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-138">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="6ea1c-139">Es stellt den Status des Antragstellers Zugriff auf die Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-139">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="6ea1c-140">Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=subjectCount` in der Abfrage.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-140">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="6ea1c-141">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="6ea1c-141">eligibleAssignmentCount</span></span>|<span data-ttu-id="6ea1c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea1c-142">Int32</span></span>|<span data-ttu-id="6ea1c-143">Optional.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-143">Optional.</span></span> <span data-ttu-id="6ea1c-144">Die Anzahl von zu auswählbaren rollenzuweisungen Rollendefinition zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-144">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="6ea1c-145">Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=eligibleAssignmentCount` in der Abfrage.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-145">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="6ea1c-146">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="6ea1c-146">activeAssignmentCount</span></span>|<span data-ttu-id="6ea1c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea1c-147">Int32</span></span>    |<span data-ttu-id="6ea1c-148">Optional.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-148">Optional.</span></span> <span data-ttu-id="6ea1c-149">Die Anzahl der aktiven rollenzuweisungen Rollendefinition zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-149">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="6ea1c-150">Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=activeAssignmentCount` in der Abfrage.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-150">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="6ea1c-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6ea1c-151">Relationships</span></span>
| <span data-ttu-id="6ea1c-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6ea1c-152">Relationship</span></span> | <span data-ttu-id="6ea1c-153">Typ</span><span class="sxs-lookup"><span data-stu-id="6ea1c-153">Type</span></span>   |<span data-ttu-id="6ea1c-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ea1c-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ea1c-155">resource</span><span class="sxs-lookup"><span data-stu-id="6ea1c-155">resource</span></span>|[<span data-ttu-id="6ea1c-156">governanceResource</span><span class="sxs-lookup"><span data-stu-id="6ea1c-156">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="6ea1c-157">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-157">Read-only.</span></span> <span data-ttu-id="6ea1c-158">Die zugeordneten Ressource für die Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-158">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="6ea1c-159">roleSetting</span><span class="sxs-lookup"><span data-stu-id="6ea1c-159">roleSetting</span></span>|[<span data-ttu-id="6ea1c-160">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="6ea1c-160">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="6ea1c-161">Die Einstellung der zugehörige Rolle für die Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-161">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ea1c-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ea1c-162">JSON representation</span></span>

<span data-ttu-id="6ea1c-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ea1c-163">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroledefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
