---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 6e20df0cf50a7fc2648f5df97fcfe84e83992d99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826194"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="ab8de-102">SharedDriveItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ab8de-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="ab8de-103">Die **sharedDriveItem**-Ressource wird zurückgegeben, wenn die [Freigabe](../api/shares-get.md)-API für den Zugriff auf ein freigegebenes[driveItem](driveitem.md)-Objekt verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="ab8de-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab8de-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ab8de-104">JSON representation</span></span>

<span data-ttu-id="ab8de-105">Es folgt eine JSON-Darstellung einer **sharedDriveItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="ab8de-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="ab8de-106">Die **sharedDriveItem**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="ab8de-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="ab8de-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ab8de-107">Properties</span></span>

| <span data-ttu-id="ab8de-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ab8de-108">Property</span></span> | <span data-ttu-id="ab8de-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ab8de-109">Type</span></span>                          | <span data-ttu-id="ab8de-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab8de-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="ab8de-111">id</span><span class="sxs-lookup"><span data-stu-id="ab8de-111">id</span></span>       | <span data-ttu-id="ab8de-112">String</span><span class="sxs-lookup"><span data-stu-id="ab8de-112">String</span></span>                        | <span data-ttu-id="ab8de-113">Die eindeutige ID der Freigabe, auf die zugegriffen wird.</span><span class="sxs-lookup"><span data-stu-id="ab8de-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="ab8de-114">name</span><span class="sxs-lookup"><span data-stu-id="ab8de-114">name</span></span>     | <span data-ttu-id="ab8de-115">String</span><span class="sxs-lookup"><span data-stu-id="ab8de-115">String</span></span>                        | <span data-ttu-id="ab8de-116">Der Anzeigename für das freigegebene Element.</span><span class="sxs-lookup"><span data-stu-id="ab8de-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="ab8de-117">owner</span><span class="sxs-lookup"><span data-stu-id="ab8de-117">owner</span></span>    | [<span data-ttu-id="ab8de-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="ab8de-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="ab8de-119">Informationen zum Besitzer des freigegebenen Elements, auf das verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="ab8de-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ab8de-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ab8de-120">Relationships</span></span>

| <span data-ttu-id="ab8de-121">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="ab8de-121">Relationship name</span></span> | <span data-ttu-id="ab8de-122">Typ</span><span class="sxs-lookup"><span data-stu-id="ab8de-122">Type</span></span>                | <span data-ttu-id="ab8de-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab8de-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="ab8de-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="ab8de-124">**driveItem**</span></span>     | <span data-ttu-id="ab8de-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="ab8de-125">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="ab8de-126">Dient für den Zugriff auf das zugrunde liegende **driveItem**</span><span class="sxs-lookup"><span data-stu-id="ab8de-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="ab8de-127">**list**</span><span class="sxs-lookup"><span data-stu-id="ab8de-127">**list**</span></span>          | <span data-ttu-id="ab8de-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="ab8de-128">[**list**][list]</span></span>        | <span data-ttu-id="ab8de-129">Dient für den Zugriff auf das zugrunde liegende **list**</span><span class="sxs-lookup"><span data-stu-id="ab8de-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="ab8de-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="ab8de-130">**listItem**</span></span>      | <span data-ttu-id="ab8de-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="ab8de-131">[**listItem**][listItem]</span></span>    | <span data-ttu-id="ab8de-132">Dient für den Zugriff auf das zugrunde liegende **listItem**</span><span class="sxs-lookup"><span data-stu-id="ab8de-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="ab8de-133">**site**</span><span class="sxs-lookup"><span data-stu-id="ab8de-133">**site**</span></span>          | <span data-ttu-id="ab8de-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="ab8de-134">[**site**][site]</span></span>        | <span data-ttu-id="ab8de-135">Dient für den Zugriff auf das zugrunde liegende **site**</span><span class="sxs-lookup"><span data-stu-id="ab8de-135">Used to access the underlying **site**</span></span>

<span data-ttu-id="ab8de-136">Für in persönlichen OneDrive-Konten freigegebene **driveItems** könnenSie alternativ ebenfalls folgende Beziehungen verwenden.</span><span class="sxs-lookup"><span data-stu-id="ab8de-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="ab8de-137">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="ab8de-137">Relationship name</span></span> | <span data-ttu-id="ab8de-138">Typ</span><span class="sxs-lookup"><span data-stu-id="ab8de-138">Type</span></span>                         | <span data-ttu-id="ab8de-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab8de-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="ab8de-140">**items**</span><span class="sxs-lookup"><span data-stu-id="ab8de-140">**items**</span></span>         | <span data-ttu-id="ab8de-141">[**driveItem**][driveItem]-Sammmlung</span><span class="sxs-lookup"><span data-stu-id="ab8de-141">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="ab8de-142">Alle im Freigabestamm enthaltenen driveItems.</span><span class="sxs-lookup"><span data-stu-id="ab8de-142">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="ab8de-143">Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="ab8de-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="ab8de-144">**root**</span><span class="sxs-lookup"><span data-stu-id="ab8de-144">**root**</span></span>          | <span data-ttu-id="ab8de-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="ab8de-145">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="ab8de-146">Verwendet, um die zugrunde liegenden **DriveItem**zugreifen.</span><span class="sxs-lookup"><span data-stu-id="ab8de-146">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="ab8de-147">Veraltet – verwenden Sie `driveItem` stattdessen.</span><span class="sxs-lookup"><span data-stu-id="ab8de-147">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="ab8de-148">Methoden</span><span class="sxs-lookup"><span data-stu-id="ab8de-148">Methods</span></span>

| <span data-ttu-id="ab8de-149">Methode</span><span class="sxs-lookup"><span data-stu-id="ab8de-149">Method</span></span>                                  | <span data-ttu-id="ab8de-150">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="ab8de-150">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="ab8de-151">Freigegebenes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="ab8de-151">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="ab8de-152">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="ab8de-152">Remarks</span></span>

<span data-ttu-id="ab8de-153">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ab8de-153">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
