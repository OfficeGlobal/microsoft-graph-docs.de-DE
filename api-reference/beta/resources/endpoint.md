---
title: Endpunkt-Ressourcentyp
description: 'Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.  Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt. Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien. Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden. Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen. '
localization_priority: Normal
ms.openlocfilehash: 5a342bee0a1918eb142542693198173239d1b3c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871284"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="72f8a-107">Endpunkt-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="72f8a-107">Endpoint resource type</span></span>

> <span data-ttu-id="72f8a-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="72f8a-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72f8a-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="72f8a-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72f8a-110">Endpunkte stellen URLs für eine Entität zugeordneten Ressourcen dar.</span><span class="sxs-lookup"><span data-stu-id="72f8a-110">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="72f8a-111">Wenn eine neue Office 365-Gruppe erstellt wird, werden zusätzliche Ressourcen beispielsweise auch als Teil der Office 365-Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="72f8a-111">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="72f8a-112">Dazu gehören Dinge wie ein Gruppenpostfach für Unterhaltungen und eine OneDrive-Ordner für Dokumente und Dateien.</span><span class="sxs-lookup"><span data-stu-id="72f8a-112">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="72f8a-113">Weitere Informationen über diese Office 365 Group-Ressourcen, einschließlich deren zugeordneten Ressource URLs kann nun mit der *Endpunkte* Navigation auf der Gruppe Ressourcentyp gelesen werden.</span><span class="sxs-lookup"><span data-stu-id="72f8a-113">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="72f8a-114">Dies ist die Anwendung zu verstehen sind diese Ressourcen, und betten die Ressource, die URL guter sogar in ihrer eigenen Erfahrungen.</span><span class="sxs-lookup"><span data-stu-id="72f8a-114">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="72f8a-115">Methoden</span><span class="sxs-lookup"><span data-stu-id="72f8a-115">Methods</span></span>

| <span data-ttu-id="72f8a-116">Methode</span><span class="sxs-lookup"><span data-stu-id="72f8a-116">Method</span></span>           | <span data-ttu-id="72f8a-117">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="72f8a-117">Return Type</span></span>    |<span data-ttu-id="72f8a-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72f8a-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72f8a-119">Endpunkte auflisten</span><span class="sxs-lookup"><span data-stu-id="72f8a-119">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="72f8a-120">[Endpunkt](endpoint.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="72f8a-120">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="72f8a-121">Rufen Sie eine Auflistung der Endpunkt-Objekts.</span><span class="sxs-lookup"><span data-stu-id="72f8a-121">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="72f8a-122">Get-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="72f8a-122">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="72f8a-123">Endpunkt</span><span class="sxs-lookup"><span data-stu-id="72f8a-123">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="72f8a-124">Lesen Sie Eigenschaften und Beziehungen eines Endpunkts-Objekts.</span><span class="sxs-lookup"><span data-stu-id="72f8a-124">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="72f8a-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="72f8a-125">Properties</span></span>
| <span data-ttu-id="72f8a-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="72f8a-126">Property</span></span>     | <span data-ttu-id="72f8a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="72f8a-127">Type</span></span>   |<span data-ttu-id="72f8a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72f8a-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="72f8a-129">Funktion</span><span class="sxs-lookup"><span data-stu-id="72f8a-129">capability</span></span>     | <span data-ttu-id="72f8a-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72f8a-130">String</span></span>  | <span data-ttu-id="72f8a-131">Beschreibt die Fähigkeit, die diese Ressource zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="72f8a-131">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="72f8a-132">(z. B. Nachrichten, Unterhaltungen, usw.)  Nicht NULL-Werte zulässt.</span><span class="sxs-lookup"><span data-stu-id="72f8a-132">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="72f8a-133">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="72f8a-133">Read-only.</span></span> |
| <span data-ttu-id="72f8a-134">id</span><span class="sxs-lookup"><span data-stu-id="72f8a-134">id</span></span>             | <span data-ttu-id="72f8a-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72f8a-135">String</span></span>  | <span data-ttu-id="72f8a-136">Eindeutiger Bezeichner für den Endpunkt; -Taste.</span><span class="sxs-lookup"><span data-stu-id="72f8a-136">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="72f8a-137">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="72f8a-137">Not nullable.</span></span> <span data-ttu-id="72f8a-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="72f8a-138">Read-only.</span></span>|
| <span data-ttu-id="72f8a-139">providerId</span><span class="sxs-lookup"><span data-stu-id="72f8a-139">providerId</span></span>     | <span data-ttu-id="72f8a-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72f8a-140">String</span></span>  | <span data-ttu-id="72f8a-141">Id der das zugrunde liegende Dienst veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="72f8a-141">Application id of the publishing underlying service.</span></span> <span data-ttu-id="72f8a-142">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="72f8a-142">Not nullable.</span></span> <span data-ttu-id="72f8a-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="72f8a-143">Read-only.</span></span>|
| <span data-ttu-id="72f8a-144">providerName</span><span class="sxs-lookup"><span data-stu-id="72f8a-144">providerName</span></span>   | <span data-ttu-id="72f8a-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72f8a-145">String</span></span>  | <span data-ttu-id="72f8a-146">Name der Veröffentlichung der zugrunde liegende Dienst.</span><span class="sxs-lookup"><span data-stu-id="72f8a-146">Name of the publishing underlying service.</span></span> <span data-ttu-id="72f8a-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="72f8a-147">Read-only.</span></span>|
| <span data-ttu-id="72f8a-148">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="72f8a-148">providerResourceId</span></span>|<span data-ttu-id="72f8a-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72f8a-149">String</span></span>| <span data-ttu-id="72f8a-150">Für Office 365-Gruppen ist dies auf einen bekannten Namen für die Ressource (z. B. Yammer.FeedURL usw.) festgelegt.</span><span class="sxs-lookup"><span data-stu-id="72f8a-150">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="72f8a-151">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="72f8a-151">Not nullable.</span></span> <span data-ttu-id="72f8a-152">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="72f8a-152">Read-only.</span></span>|
| <span data-ttu-id="72f8a-153">uri</span><span class="sxs-lookup"><span data-stu-id="72f8a-153">uri</span></span>            | <span data-ttu-id="72f8a-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72f8a-154">String</span></span>  | <span data-ttu-id="72f8a-155">URL der veröffentlichten Ressource.</span><span class="sxs-lookup"><span data-stu-id="72f8a-155">URL of the published resource.</span></span> <span data-ttu-id="72f8a-156">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="72f8a-156">Not nullable.</span></span> <span data-ttu-id="72f8a-157">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="72f8a-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72f8a-158">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="72f8a-158">Relationships</span></span>

<span data-ttu-id="72f8a-159">Keine.</span><span class="sxs-lookup"><span data-stu-id="72f8a-159">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="72f8a-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="72f8a-160">JSON representation</span></span>
<span data-ttu-id="72f8a-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="72f8a-161">Here is a JSON representation of the resource.</span></span>

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
