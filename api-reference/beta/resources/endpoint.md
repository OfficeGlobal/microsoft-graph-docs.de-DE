---
title: Endpunkt-Ressourcentyp
description: 'Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.  Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt. Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien. Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden. Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen. '
localization_priority: Normal
ms.openlocfilehash: 39a6a2d8213e809f426c492654272aa994c25a6d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574482"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="bdf15-107">Endpunkt-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bdf15-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf15-108">Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.</span><span class="sxs-lookup"><span data-stu-id="bdf15-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="bdf15-109">Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="bdf15-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="bdf15-110">Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien.</span><span class="sxs-lookup"><span data-stu-id="bdf15-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="bdf15-111">Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden.</span><span class="sxs-lookup"><span data-stu-id="bdf15-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="bdf15-112">Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen.</span><span class="sxs-lookup"><span data-stu-id="bdf15-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="bdf15-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="bdf15-113">Methods</span></span>

| <span data-ttu-id="bdf15-114">Methode</span><span class="sxs-lookup"><span data-stu-id="bdf15-114">Method</span></span>           | <span data-ttu-id="bdf15-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bdf15-115">Return Type</span></span>    |<span data-ttu-id="bdf15-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdf15-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bdf15-117">Endpunkte auflisten</span><span class="sxs-lookup"><span data-stu-id="bdf15-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="bdf15-118">[endpoint](endpoint.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bdf15-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="bdf15-119">Ruft eine Endpunktobjektsammlung ab.</span><span class="sxs-lookup"><span data-stu-id="bdf15-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="bdf15-120">Endpunkt abrufen</span><span class="sxs-lookup"><span data-stu-id="bdf15-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="bdf15-121">Endpunkt</span><span class="sxs-lookup"><span data-stu-id="bdf15-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="bdf15-122">Dient zum Lesen der Eigenschaften und der Beziehungen des endpoint-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bdf15-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bdf15-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bdf15-123">Properties</span></span>
| <span data-ttu-id="bdf15-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bdf15-124">Property</span></span>     | <span data-ttu-id="bdf15-125">Typ</span><span class="sxs-lookup"><span data-stu-id="bdf15-125">Type</span></span>   |<span data-ttu-id="bdf15-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdf15-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bdf15-127">Funktion</span><span class="sxs-lookup"><span data-stu-id="bdf15-127">capability</span></span>     | <span data-ttu-id="bdf15-128">String</span><span class="sxs-lookup"><span data-stu-id="bdf15-128">String</span></span>  | <span data-ttu-id="bdf15-129">Beschreibt die Fähigkeit, die diese Ressource zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="bdf15-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="bdf15-130">(z. B. Nachrichten, Unterhaltungen, usw.)  Nicht NULL-Werte zulässt.</span><span class="sxs-lookup"><span data-stu-id="bdf15-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="bdf15-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bdf15-131">Read-only.</span></span> |
| <span data-ttu-id="bdf15-132">id</span><span class="sxs-lookup"><span data-stu-id="bdf15-132">id</span></span>             | <span data-ttu-id="bdf15-133">String</span><span class="sxs-lookup"><span data-stu-id="bdf15-133">String</span></span>  | <span data-ttu-id="bdf15-134">Eindeutiger Bezeichner für den Endpunkt; -Taste.</span><span class="sxs-lookup"><span data-stu-id="bdf15-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="bdf15-135">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="bdf15-135">Not nullable.</span></span> <span data-ttu-id="bdf15-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bdf15-136">Read-only.</span></span>|
| <span data-ttu-id="bdf15-137">providerId</span><span class="sxs-lookup"><span data-stu-id="bdf15-137">providerId</span></span>     | <span data-ttu-id="bdf15-138">String</span><span class="sxs-lookup"><span data-stu-id="bdf15-138">String</span></span>  | <span data-ttu-id="bdf15-139">Id der das zugrunde liegende Dienst veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="bdf15-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="bdf15-140">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="bdf15-140">Not nullable.</span></span> <span data-ttu-id="bdf15-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bdf15-141">Read-only.</span></span>|
| <span data-ttu-id="bdf15-142">providerName</span><span class="sxs-lookup"><span data-stu-id="bdf15-142">providerName</span></span>   | <span data-ttu-id="bdf15-143">String</span><span class="sxs-lookup"><span data-stu-id="bdf15-143">String</span></span>  | <span data-ttu-id="bdf15-144">Name der Veröffentlichung der zugrunde liegende Dienst.</span><span class="sxs-lookup"><span data-stu-id="bdf15-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="bdf15-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bdf15-145">Read-only.</span></span>|
| <span data-ttu-id="bdf15-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="bdf15-146">providerResourceId</span></span>|<span data-ttu-id="bdf15-147">String</span><span class="sxs-lookup"><span data-stu-id="bdf15-147">String</span></span>| <span data-ttu-id="bdf15-148">Für Office 365-Gruppen ist dies auf einen bekannten Namen für die Ressource (z. B. Yammer.FeedURL usw.) festgelegt.</span><span class="sxs-lookup"><span data-stu-id="bdf15-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="bdf15-149">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="bdf15-149">Not nullable.</span></span> <span data-ttu-id="bdf15-150">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bdf15-150">Read-only.</span></span>|
| <span data-ttu-id="bdf15-151">uri</span><span class="sxs-lookup"><span data-stu-id="bdf15-151">uri</span></span>            | <span data-ttu-id="bdf15-152">String</span><span class="sxs-lookup"><span data-stu-id="bdf15-152">String</span></span>  | <span data-ttu-id="bdf15-153">URL der veröffentlichten Ressource.</span><span class="sxs-lookup"><span data-stu-id="bdf15-153">URL of the published resource.</span></span> <span data-ttu-id="bdf15-154">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="bdf15-154">Not nullable.</span></span> <span data-ttu-id="bdf15-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bdf15-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdf15-156">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bdf15-156">Relationships</span></span>

<span data-ttu-id="bdf15-157">Keine.</span><span class="sxs-lookup"><span data-stu-id="bdf15-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bdf15-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bdf15-158">JSON representation</span></span>
<span data-ttu-id="bdf15-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bdf15-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.endpoint"
}-->

```json
{
  "capability": "String",
  "id": "String (identifier)",
  "providerId": "String",
  "providerName": "String",
  "providerResourceId": "String",
  "uri": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
