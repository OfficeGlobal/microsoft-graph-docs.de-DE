---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
ms.openlocfilehash: 3b4497c1a15704388dbb4bb4ba181d3985d65a69
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="bee7f-102">sharedDriveItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bee7f-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="bee7f-103">Die **sharedDriveItem**-Ressource wird zurückgegeben, wenn die [Freigabe](../api/shares_get.md)-API für den Zugriff auf ein freigegebenes[driveItem](driveitem.md)-Objekt verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="bee7f-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares_get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bee7f-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bee7f-104">JSON representation</span></span>

<span data-ttu-id="bee7f-105">Es folgt eine JSON-Darstellung einer **sharedDriveItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="bee7f-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="bee7f-106">Die **sharedDriveItem**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="bee7f-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="bee7f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bee7f-107">Properties</span></span>

| <span data-ttu-id="bee7f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bee7f-108">Property</span></span> | <span data-ttu-id="bee7f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bee7f-109">Type</span></span>                          | <span data-ttu-id="bee7f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bee7f-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="bee7f-111">id</span><span class="sxs-lookup"><span data-stu-id="bee7f-111">id</span></span>       | <span data-ttu-id="bee7f-112">String</span><span class="sxs-lookup"><span data-stu-id="bee7f-112">String</span></span>                        | <span data-ttu-id="bee7f-113">Die eindeutige ID der Freigabe, auf die zugegriffen wird.</span><span class="sxs-lookup"><span data-stu-id="bee7f-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="bee7f-114">name</span><span class="sxs-lookup"><span data-stu-id="bee7f-114">name</span></span>     | <span data-ttu-id="bee7f-115">String</span><span class="sxs-lookup"><span data-stu-id="bee7f-115">String</span></span>                        | <span data-ttu-id="bee7f-116">Der Anzeigename für das freigegebene Element.</span><span class="sxs-lookup"><span data-stu-id="bee7f-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="bee7f-117">owner</span><span class="sxs-lookup"><span data-stu-id="bee7f-117">owner</span></span>    | [<span data-ttu-id="bee7f-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="bee7f-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="bee7f-119">Informationen zum Besitzer des freigegebenen Elements, auf das verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="bee7f-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bee7f-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bee7f-120">Relationships</span></span>

| <span data-ttu-id="bee7f-121">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="bee7f-121">Relationship name</span></span> | <span data-ttu-id="bee7f-122">Typ</span><span class="sxs-lookup"><span data-stu-id="bee7f-122">Type</span></span>                | <span data-ttu-id="bee7f-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bee7f-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="bee7f-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="bee7f-124">**DriveItem**</span></span>     | <span data-ttu-id="bee7f-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="bee7f-125">DriveItem</span></span>   | <span data-ttu-id="bee7f-126">Dient für den Zugriff auf das zugrunde liegende **driveItem**</span><span class="sxs-lookup"><span data-stu-id="bee7f-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="bee7f-127">**list**</span><span class="sxs-lookup"><span data-stu-id="bee7f-127">**list**</span></span>          | <span data-ttu-id="bee7f-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="bee7f-128">List</span></span>        | <span data-ttu-id="bee7f-129">Dient für den Zugriff auf die zugrunde liegende **list**</span><span class="sxs-lookup"><span data-stu-id="bee7f-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="bee7f-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="bee7f-130">**listItem**</span></span>      | <span data-ttu-id="bee7f-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="bee7f-131">**ListItem**</span></span>    | <span data-ttu-id="bee7f-132">Dient für den Zugriff auf das zugrunde liegende **listItem**</span><span class="sxs-lookup"><span data-stu-id="bee7f-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="bee7f-133">**site**</span><span class="sxs-lookup"><span data-stu-id="bee7f-133">**site**</span></span>          | <span data-ttu-id="bee7f-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="bee7f-134">**site**</span></span>        | <span data-ttu-id="bee7f-135">Dient für den Zugriff auf die zugrunde liegende **site**</span><span class="sxs-lookup"><span data-stu-id="bee7f-135">Used to access the underlying **site**</span></span>


<span data-ttu-id="bee7f-136">Für in persönlichen OneDrive-Konten freigegebene **driveItems** können Sie alternativ ebenfalls folgende Beziehungen verwenden.</span><span class="sxs-lookup"><span data-stu-id="bee7f-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="bee7f-137">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="bee7f-137">Relationship name</span></span> | <span data-ttu-id="bee7f-138">Typ</span><span class="sxs-lookup"><span data-stu-id="bee7f-138">Type</span></span>                         | <span data-ttu-id="bee7f-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bee7f-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="bee7f-140">**items**</span><span class="sxs-lookup"><span data-stu-id="bee7f-140">**items**</span></span>         | <span data-ttu-id="bee7f-141">[**driveItem**][driveItem]-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bee7f-141">**driveItem** collection</span></span> | <span data-ttu-id="bee7f-142">Alle im Freigabestamm enthaltenen driveItems.</span><span class="sxs-lookup"><span data-stu-id="bee7f-142">All items contained in the sharing root.</span></span> <span data-ttu-id="bee7f-143">Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="bee7f-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="bee7f-144">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="bee7f-144">**DriveItem**</span></span>     | <span data-ttu-id="bee7f-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="bee7f-145">DriveItem</span></span>            | <span data-ttu-id="bee7f-146">Dient für den Zugriff auf das zugrunde liegende **driveItem**</span><span class="sxs-lookup"><span data-stu-id="bee7f-146">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveItem.md
[list]: list.md
[listItem]: listItem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="bee7f-147">Methoden</span><span class="sxs-lookup"><span data-stu-id="bee7f-147">Methods</span></span>

| <span data-ttu-id="bee7f-148">Method</span><span class="sxs-lookup"><span data-stu-id="bee7f-148">Method</span></span>                                  | <span data-ttu-id="bee7f-149">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="bee7f-149">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="bee7f-150">Freigegebenes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="bee7f-150">Get shared item</span></span>](../api/shares_get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="bee7f-151">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="bee7f-151">Remarks</span></span>

<span data-ttu-id="bee7f-152">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="bee7f-152">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
