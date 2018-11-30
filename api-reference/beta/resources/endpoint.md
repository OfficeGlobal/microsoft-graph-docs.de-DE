---
title: Endpunkt-Ressourcentyp
description: 'Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.  Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt. Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien. Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden. Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen. '
ms.openlocfilehash: 8d95cef8e25095512e94d5aed5ec7540562862bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059776"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="4e1d7-107">Endpunkt-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4e1d7-107">Endpoint resource type</span></span>

> <span data-ttu-id="4e1d7-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e1d7-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e1d7-110">Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-110">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="4e1d7-111">Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-111">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="4e1d7-112">Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-112">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="4e1d7-113">Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-113">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="4e1d7-114">Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-114">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="4e1d7-115">Methoden</span><span class="sxs-lookup"><span data-stu-id="4e1d7-115">Methods</span></span>

| <span data-ttu-id="4e1d7-116">Methode</span><span class="sxs-lookup"><span data-stu-id="4e1d7-116">Method</span></span>           | <span data-ttu-id="4e1d7-117">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4e1d7-117">Return Type</span></span>    |<span data-ttu-id="4e1d7-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e1d7-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e1d7-119">Endpunkte auflisten</span><span class="sxs-lookup"><span data-stu-id="4e1d7-119">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="4e1d7-120">[Endpunkt](endpoint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4e1d7-120">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="4e1d7-121">Rufen Sie eine Auflistung der Endpunkt-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-121">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="4e1d7-122">Get-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="4e1d7-122">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="4e1d7-123">Endpunkt</span><span class="sxs-lookup"><span data-stu-id="4e1d7-123">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="4e1d7-124">Lesen Sie Eigenschaften und Beziehungen eines Endpunkts-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-124">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e1d7-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4e1d7-125">Properties</span></span>
| <span data-ttu-id="4e1d7-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e1d7-126">Property</span></span>     | <span data-ttu-id="4e1d7-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4e1d7-127">Type</span></span>   |<span data-ttu-id="4e1d7-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e1d7-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4e1d7-129">Funktion</span><span class="sxs-lookup"><span data-stu-id="4e1d7-129">capability</span></span>     | <span data-ttu-id="4e1d7-130">String</span><span class="sxs-lookup"><span data-stu-id="4e1d7-130">String</span></span>  | <span data-ttu-id="4e1d7-131">Beschreibt die Fähigkeit, die diese Ressource zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-131">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="4e1d7-132">(z. B. Nachrichten, Unterhaltungen, usw.)  Nicht NULL-Werte zulässt.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-132">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="4e1d7-133">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-133">Read-only.</span></span> |
| <span data-ttu-id="4e1d7-134">id</span><span class="sxs-lookup"><span data-stu-id="4e1d7-134">id</span></span>             | <span data-ttu-id="4e1d7-135">String</span><span class="sxs-lookup"><span data-stu-id="4e1d7-135">String</span></span>  | <span data-ttu-id="4e1d7-136">Eindeutiger Bezeichner für den Endpunkt; -Taste.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-136">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="4e1d7-137">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-137">Not nullable.</span></span> <span data-ttu-id="4e1d7-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-138">Read-only.</span></span>|
| <span data-ttu-id="4e1d7-139">providerId</span><span class="sxs-lookup"><span data-stu-id="4e1d7-139">providerId</span></span>     | <span data-ttu-id="4e1d7-140">String</span><span class="sxs-lookup"><span data-stu-id="4e1d7-140">String</span></span>  | <span data-ttu-id="4e1d7-141">Id der das zugrunde liegende Dienst veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-141">Application id of the publishing underlying service.</span></span> <span data-ttu-id="4e1d7-142">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-142">Not nullable.</span></span> <span data-ttu-id="4e1d7-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-143">Read-only.</span></span>|
| <span data-ttu-id="4e1d7-144">providerName</span><span class="sxs-lookup"><span data-stu-id="4e1d7-144">providerName</span></span>   | <span data-ttu-id="4e1d7-145">String</span><span class="sxs-lookup"><span data-stu-id="4e1d7-145">String</span></span>  | <span data-ttu-id="4e1d7-146">Name der Veröffentlichung der zugrunde liegende Dienst.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-146">Name of the publishing underlying service.</span></span> <span data-ttu-id="4e1d7-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-147">Read-only.</span></span>|
| <span data-ttu-id="4e1d7-148">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="4e1d7-148">providerResourceId</span></span>|<span data-ttu-id="4e1d7-149">String</span><span class="sxs-lookup"><span data-stu-id="4e1d7-149">String</span></span>| <span data-ttu-id="4e1d7-150">Für Office 365-Gruppen ist dies auf einen bekannten Namen für die Ressource (z. B. Yammer.FeedURL usw.) festgelegt.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-150">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="4e1d7-151">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-151">Not nullable.</span></span> <span data-ttu-id="4e1d7-152">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-152">Read-only.</span></span>|
| <span data-ttu-id="4e1d7-153">uri</span><span class="sxs-lookup"><span data-stu-id="4e1d7-153">uri</span></span>            | <span data-ttu-id="4e1d7-154">String</span><span class="sxs-lookup"><span data-stu-id="4e1d7-154">String</span></span>  | <span data-ttu-id="4e1d7-155">URL der veröffentlichten Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-155">URL of the published resource.</span></span> <span data-ttu-id="4e1d7-156">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-156">Not nullable.</span></span> <span data-ttu-id="4e1d7-157">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e1d7-158">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4e1d7-158">Relationships</span></span>

<span data-ttu-id="4e1d7-159">Keine.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-159">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4e1d7-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4e1d7-160">JSON representation</span></span>
<span data-ttu-id="4e1d7-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e1d7-161">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->