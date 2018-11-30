---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
ms.openlocfilehash: 44d8a7c2bab9f19ff7b7680aea2e2a88fc2ef245
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058202"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="bc1e7-102">SharedDriveItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bc1e7-102">SharedDriveItem resource type</span></span>

> <span data-ttu-id="bc1e7-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc1e7-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc1e7-105">Die **sharedDriveItem**-Ressource wird zurückgegeben, wenn die [Freigabe](../api/shares-get.md)-API für den Zugriff auf ein freigegebenes[driveItem](driveitem.md)-Objekt verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc1e7-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bc1e7-106">JSON representation</span></span>

<span data-ttu-id="bc1e7-107">Es folgt eine JSON-Darstellung einer **sharedDriveItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="bc1e7-108">Die **sharedDriveItem**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "permission": { "@odata.type": "microsoft.graph.permission" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="bc1e7-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc1e7-109">Properties</span></span>

| <span data-ttu-id="bc1e7-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc1e7-110">Property</span></span> | <span data-ttu-id="bc1e7-111">Typ</span><span class="sxs-lookup"><span data-stu-id="bc1e7-111">Type</span></span>                          | <span data-ttu-id="bc1e7-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc1e7-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="bc1e7-113">id</span><span class="sxs-lookup"><span data-stu-id="bc1e7-113">id</span></span>       | <span data-ttu-id="bc1e7-114">String</span><span class="sxs-lookup"><span data-stu-id="bc1e7-114">String</span></span>                        | <span data-ttu-id="bc1e7-115">Die eindeutige ID der Freigabe, auf die zugegriffen wird.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="bc1e7-116">name</span><span class="sxs-lookup"><span data-stu-id="bc1e7-116">name</span></span>     | <span data-ttu-id="bc1e7-117">String</span><span class="sxs-lookup"><span data-stu-id="bc1e7-117">String</span></span>                        | <span data-ttu-id="bc1e7-118">Der Anzeigename für das freigegebene Element.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="bc1e7-119">owner</span><span class="sxs-lookup"><span data-stu-id="bc1e7-119">owner</span></span>    | [<span data-ttu-id="bc1e7-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="bc1e7-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="bc1e7-121">Informationen zum Besitzer des freigegebenen Elements, auf das verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bc1e7-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bc1e7-122">Relationships</span></span>

| <span data-ttu-id="bc1e7-123">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="bc1e7-123">Relationship name</span></span> | <span data-ttu-id="bc1e7-124">Typ</span><span class="sxs-lookup"><span data-stu-id="bc1e7-124">Type</span></span>                | <span data-ttu-id="bc1e7-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc1e7-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="bc1e7-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-126">**driveItem**</span></span>     | <span data-ttu-id="bc1e7-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="bc1e7-127">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="bc1e7-128">Dient für den Zugriff auf das zugrunde liegende **driveItem**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="bc1e7-129">**list**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-129">**list**</span></span>          | <span data-ttu-id="bc1e7-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="bc1e7-130">[**list**][list]</span></span>           | <span data-ttu-id="bc1e7-131">Dient für den Zugriff auf das zugrunde liegende **list**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="bc1e7-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-132">**listItem**</span></span>      | <span data-ttu-id="bc1e7-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="bc1e7-133">[**listItem**][listItem]</span></span>   | <span data-ttu-id="bc1e7-134">Dient für den Zugriff auf das zugrunde liegende **listItem**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="bc1e7-135">**permission**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-135">**permission**</span></span>    | <span data-ttu-id="bc1e7-136">[**Berechtigung**][permission]</span><span class="sxs-lookup"><span data-stu-id="bc1e7-136">[**permission**][permission]</span></span> | <span data-ttu-id="bc1e7-137">Verwendet, um die **Berechtigung** für den zugrunde liegenden sharing Hyperlink zugreifen</span><span class="sxs-lookup"><span data-stu-id="bc1e7-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="bc1e7-138">**site**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-138">**site**</span></span>          | <span data-ttu-id="bc1e7-139">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="bc1e7-139">[**site**][site]</span></span>           | <span data-ttu-id="bc1e7-140">Dient für den Zugriff auf das zugrunde liegende **site**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="bc1e7-141">Für in persönlichen OneDrive-Konten freigegebene **driveItems** könnenSie alternativ ebenfalls folgende Beziehungen verwenden.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="bc1e7-142">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="bc1e7-142">Relationship name</span></span> | <span data-ttu-id="bc1e7-143">Typ</span><span class="sxs-lookup"><span data-stu-id="bc1e7-143">Type</span></span>                         | <span data-ttu-id="bc1e7-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc1e7-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="bc1e7-145">**items**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-145">**items**</span></span>         | <span data-ttu-id="bc1e7-146">[**driveItem**][driveItem]-Sammmlung</span><span class="sxs-lookup"><span data-stu-id="bc1e7-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="bc1e7-147">Alle im Freigabestamm enthaltenen driveItems.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="bc1e7-148">Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="bc1e7-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="bc1e7-149">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-149">**driveItem**</span></span>     | <span data-ttu-id="bc1e7-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="bc1e7-150">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="bc1e7-151">Dient für den Zugriff auf das zugrunde liegende **driveItem**</span><span class="sxs-lookup"><span data-stu-id="bc1e7-151">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="bc1e7-152">Methoden</span><span class="sxs-lookup"><span data-stu-id="bc1e7-152">Methods</span></span>

| <span data-ttu-id="bc1e7-153">Methode</span><span class="sxs-lookup"><span data-stu-id="bc1e7-153">Method</span></span>                                  | <span data-ttu-id="bc1e7-154">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="bc1e7-154">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="bc1e7-155">Freigegebenes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="bc1e7-155">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="bc1e7-156">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="bc1e7-156">Remarks</span></span>

<span data-ttu-id="bc1e7-157">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="bc1e7-157">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
