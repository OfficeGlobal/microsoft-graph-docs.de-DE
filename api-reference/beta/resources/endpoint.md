---
title: Endpunkt-Ressourcentyp
description: 'Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.  Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt. Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien. Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden. Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen. '
localization_priority: Normal
ms.openlocfilehash: 6f923cdeb34ec0845d776a67f51db490256ec718
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512059"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="0f8cd-107">Endpunkt-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0f8cd-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f8cd-108">Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="0f8cd-109">Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="0f8cd-110">Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="0f8cd-111">Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="0f8cd-112">Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="0f8cd-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="0f8cd-113">Methods</span></span>

| <span data-ttu-id="0f8cd-114">Methode</span><span class="sxs-lookup"><span data-stu-id="0f8cd-114">Method</span></span>           | <span data-ttu-id="0f8cd-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0f8cd-115">Return Type</span></span>    |<span data-ttu-id="0f8cd-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f8cd-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f8cd-117">Endpunkte auflisten</span><span class="sxs-lookup"><span data-stu-id="0f8cd-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="0f8cd-118">[endpoint](endpoint.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0f8cd-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="0f8cd-119">Ruft eine Endpunktobjektsammlung ab.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="0f8cd-120">Endpunkt abrufen</span><span class="sxs-lookup"><span data-stu-id="0f8cd-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="0f8cd-121">Endpunkt</span><span class="sxs-lookup"><span data-stu-id="0f8cd-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="0f8cd-122">Dient zum Lesen der Eigenschaften und der Beziehungen des endpoint-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f8cd-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f8cd-123">Properties</span></span>
| <span data-ttu-id="0f8cd-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f8cd-124">Property</span></span>     | <span data-ttu-id="0f8cd-125">Typ</span><span class="sxs-lookup"><span data-stu-id="0f8cd-125">Type</span></span>   |<span data-ttu-id="0f8cd-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f8cd-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0f8cd-127">Funktion</span><span class="sxs-lookup"><span data-stu-id="0f8cd-127">capability</span></span>     | <span data-ttu-id="0f8cd-128">String</span><span class="sxs-lookup"><span data-stu-id="0f8cd-128">String</span></span>  | <span data-ttu-id="0f8cd-129">Beschreibt die Fähigkeit, die diese Ressource zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="0f8cd-130">(z. B. Nachrichten, Unterhaltungen, usw.)  Nicht NULL-Werte zulässt.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="0f8cd-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-131">Read-only.</span></span> |
| <span data-ttu-id="0f8cd-132">id</span><span class="sxs-lookup"><span data-stu-id="0f8cd-132">id</span></span>             | <span data-ttu-id="0f8cd-133">String</span><span class="sxs-lookup"><span data-stu-id="0f8cd-133">String</span></span>  | <span data-ttu-id="0f8cd-134">Eindeutiger Bezeichner für den Endpunkt; -Taste.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="0f8cd-135">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-135">Not nullable.</span></span> <span data-ttu-id="0f8cd-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-136">Read-only.</span></span>|
| <span data-ttu-id="0f8cd-137">providerId</span><span class="sxs-lookup"><span data-stu-id="0f8cd-137">providerId</span></span>     | <span data-ttu-id="0f8cd-138">String</span><span class="sxs-lookup"><span data-stu-id="0f8cd-138">String</span></span>  | <span data-ttu-id="0f8cd-139">Id der das zugrunde liegende Dienst veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="0f8cd-140">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-140">Not nullable.</span></span> <span data-ttu-id="0f8cd-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-141">Read-only.</span></span>|
| <span data-ttu-id="0f8cd-142">ProviderName</span><span class="sxs-lookup"><span data-stu-id="0f8cd-142">providerName</span></span>   | <span data-ttu-id="0f8cd-143">String</span><span class="sxs-lookup"><span data-stu-id="0f8cd-143">String</span></span>  | <span data-ttu-id="0f8cd-144">Name der Veröffentlichung der zugrunde liegende Dienst.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="0f8cd-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-145">Read-only.</span></span>|
| <span data-ttu-id="0f8cd-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="0f8cd-146">providerResourceId</span></span>|<span data-ttu-id="0f8cd-147">String</span><span class="sxs-lookup"><span data-stu-id="0f8cd-147">String</span></span>| <span data-ttu-id="0f8cd-148">Für Office 365-Gruppen ist dies auf einen bekannten Namen für die Ressource (z. B. Yammer.FeedURL usw.) festgelegt.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="0f8cd-149">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-149">Not nullable.</span></span> <span data-ttu-id="0f8cd-150">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-150">Read-only.</span></span>|
| <span data-ttu-id="0f8cd-151">uri</span><span class="sxs-lookup"><span data-stu-id="0f8cd-151">uri</span></span>            | <span data-ttu-id="0f8cd-152">String</span><span class="sxs-lookup"><span data-stu-id="0f8cd-152">String</span></span>  | <span data-ttu-id="0f8cd-153">URL der veröffentlichten Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-153">URL of the published resource.</span></span> <span data-ttu-id="0f8cd-154">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-154">Not nullable.</span></span> <span data-ttu-id="0f8cd-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f8cd-156">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f8cd-156">Relationships</span></span>

<span data-ttu-id="0f8cd-157">Keine.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0f8cd-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f8cd-158">JSON representation</span></span>
<span data-ttu-id="0f8cd-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f8cd-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Endpoint"
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
