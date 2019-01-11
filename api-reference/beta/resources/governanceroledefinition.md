---
title: Ressourcentyp governanceRoleDefinition
description: Stellt die Rollendefinitionen. Für Azure Ressourcen können sie Azure RBAC-Rollen, wie Besitzer, Leser, Autor darstellen.
localization_priority: Normal
ms.openlocfilehash: 3f94dd1a741545760951875fbc064307823a65dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842450"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="1e12b-104">Ressourcentyp governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1e12b-104">governanceRoleDefinition resource type</span></span>

> <span data-ttu-id="1e12b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1e12b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e12b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e12b-106">Use of these APIs in production applications is not supported.</span></span> 


<span data-ttu-id="1e12b-107">Stellt die Rollendefinitionen.</span><span class="sxs-lookup"><span data-stu-id="1e12b-107">Represents the role definitions.</span></span> <span data-ttu-id="1e12b-108">Für Azure Ressourcen können sie Azure RBAC-Rollen, wie Besitzer, Leser, Autor darstellen.</span><span class="sxs-lookup"><span data-stu-id="1e12b-108">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="1e12b-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="1e12b-109">Methods</span></span>

| <span data-ttu-id="1e12b-110">Methode</span><span class="sxs-lookup"><span data-stu-id="1e12b-110">Method</span></span>          | <span data-ttu-id="1e12b-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1e12b-111">Return Type</span></span> |<span data-ttu-id="1e12b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e12b-112">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="1e12b-113">List</span><span class="sxs-lookup"><span data-stu-id="1e12b-113">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="1e12b-114">[GovernanceRoleDefinition](../resources/governanceroledefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="1e12b-114">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="1e12b-115">Eine Auflistung von Rollendefinitionen für eine Ressource aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="1e12b-115">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="1e12b-116">Get</span><span class="sxs-lookup"><span data-stu-id="1e12b-116">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="1e12b-117">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1e12b-117">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="1e12b-118">Lesen Sie Eigenschaften und Beziehungen einer Rolle Definition Entität nach Id angegeben.</span><span class="sxs-lookup"><span data-stu-id="1e12b-118">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="1e12b-119">Nicht `POST`, `PUT`, `PATCH`, `DELETE` wird auf unterstützt `roleDefinitions` Entität-Set für jetzt.</span><span class="sxs-lookup"><span data-stu-id="1e12b-119">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="1e12b-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1e12b-120">Properties</span></span>
| <span data-ttu-id="1e12b-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e12b-121">Property</span></span>  | <span data-ttu-id="1e12b-122">Typ</span><span class="sxs-lookup"><span data-stu-id="1e12b-122">Type</span></span>      |<span data-ttu-id="1e12b-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e12b-123">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="1e12b-124">id</span><span class="sxs-lookup"><span data-stu-id="1e12b-124">id</span></span>         |<span data-ttu-id="1e12b-125">String</span><span class="sxs-lookup"><span data-stu-id="1e12b-125">String</span></span>     |<span data-ttu-id="1e12b-126">Die Id der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="1e12b-126">The id of the role definition.</span></span> |
|<span data-ttu-id="1e12b-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="1e12b-127">resourceId</span></span> |<span data-ttu-id="1e12b-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e12b-128">String</span></span>     |<span data-ttu-id="1e12b-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1e12b-129">Required.</span></span> <span data-ttu-id="1e12b-130">Die Id der Rollendefinition zugeordneten Ressource.</span><span class="sxs-lookup"><span data-stu-id="1e12b-130">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="1e12b-131">externalId</span><span class="sxs-lookup"><span data-stu-id="1e12b-131">externalId</span></span>   |<span data-ttu-id="1e12b-132">String</span><span class="sxs-lookup"><span data-stu-id="1e12b-132">String</span></span>     |<span data-ttu-id="1e12b-133">Die externe Id der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="1e12b-133">The external id of the role definition.</span></span>|
|<span data-ttu-id="1e12b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1e12b-134">displayName</span></span>|<span data-ttu-id="1e12b-135">String</span><span class="sxs-lookup"><span data-stu-id="1e12b-135">String</span></span>     |<span data-ttu-id="1e12b-136">Der Anzeigename der Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="1e12b-136">The display name of the role definition.</span></span>|
|<span data-ttu-id="1e12b-137">subjectCount</span><span class="sxs-lookup"><span data-stu-id="1e12b-137">subjectCount</span></span>|<span data-ttu-id="1e12b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1e12b-138">Int32</span></span>     |<span data-ttu-id="1e12b-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="1e12b-139">Optional.</span></span> <span data-ttu-id="1e12b-140">Die Anzahl der Themen, die die Rolle zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="1e12b-140">The number of subjects that are assigned to the role.</span></span> <span data-ttu-id="1e12b-141">Es stellt den Status des Antragstellers Zugriff auf die Ressource.</span><span class="sxs-lookup"><span data-stu-id="1e12b-141">It represents the status of the requestor's access to the resource.</span></span> <span data-ttu-id="1e12b-142">Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=subjectCount` in der Abfrage.</span><span class="sxs-lookup"><span data-stu-id="1e12b-142">To get the property, please explictly use `$select=subjectCount` in the query.</span></span>|
|<span data-ttu-id="1e12b-143">eligibleAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="1e12b-143">eligibleAssignmentCount</span></span>|<span data-ttu-id="1e12b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="1e12b-144">Int32</span></span>|<span data-ttu-id="1e12b-145">Optional.</span><span class="sxs-lookup"><span data-stu-id="1e12b-145">Optional.</span></span> <span data-ttu-id="1e12b-146">Die Anzahl von zu auswählbaren rollenzuweisungen Rollendefinition zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="1e12b-146">The number of eligible role assignments associated with the role definition.</span></span> <span data-ttu-id="1e12b-147">Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=eligibleAssignmentCount` in der Abfrage.</span><span class="sxs-lookup"><span data-stu-id="1e12b-147">To get the property, please explictly use `$select=eligibleAssignmentCount` in the query.</span></span>|
|<span data-ttu-id="1e12b-148">activeAssignmentCount</span><span class="sxs-lookup"><span data-stu-id="1e12b-148">activeAssignmentCount</span></span>|<span data-ttu-id="1e12b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1e12b-149">Int32</span></span>    |<span data-ttu-id="1e12b-150">Optional.</span><span class="sxs-lookup"><span data-stu-id="1e12b-150">Optional.</span></span> <span data-ttu-id="1e12b-151">Die Anzahl der aktiven rollenzuweisungen Rollendefinition zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="1e12b-151">The number of active role assignments associated with the role definition.</span></span>  <span data-ttu-id="1e12b-152">Wenn die Eigenschaft erhalten möchten, geben Sie explizit labeltags verwenden `$select=activeAssignmentCount` in der Abfrage.</span><span class="sxs-lookup"><span data-stu-id="1e12b-152">To get the property, please explictly use `$select=activeAssignmentCount` in the query.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1e12b-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1e12b-153">Relationships</span></span>
| <span data-ttu-id="1e12b-154">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1e12b-154">Relationship</span></span> | <span data-ttu-id="1e12b-155">Typ</span><span class="sxs-lookup"><span data-stu-id="1e12b-155">Type</span></span>   |<span data-ttu-id="1e12b-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e12b-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e12b-157">resource</span><span class="sxs-lookup"><span data-stu-id="1e12b-157">resource</span></span>|[<span data-ttu-id="1e12b-158">governanceResource</span><span class="sxs-lookup"><span data-stu-id="1e12b-158">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="1e12b-159">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1e12b-159">Read-only.</span></span> <span data-ttu-id="1e12b-160">Die zugeordneten Ressource für die Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="1e12b-160">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="1e12b-161">roleSetting</span><span class="sxs-lookup"><span data-stu-id="1e12b-161">roleSetting</span></span>|[<span data-ttu-id="1e12b-162">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="1e12b-162">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="1e12b-163">Die Einstellung der zugehörige Rolle für die Rollendefinition.</span><span class="sxs-lookup"><span data-stu-id="1e12b-163">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e12b-164">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1e12b-164">JSON representation</span></span>

<span data-ttu-id="1e12b-165">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1e12b-165">Here is a JSON representation of the resource.</span></span>

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
