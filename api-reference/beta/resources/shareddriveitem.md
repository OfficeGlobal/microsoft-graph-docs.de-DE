---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: d20656351725f23d4fd4c00b65fdc88fe2f449b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853067"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="346b0-102">SharedDriveItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="346b0-102">SharedDriveItem resource type</span></span>

> <span data-ttu-id="346b0-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="346b0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="346b0-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="346b0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="346b0-105">Die **sharedDriveItem**-Ressource wird zurückgegeben, wenn die [Freigabe](../api/shares-get.md)-API für den Zugriff auf ein freigegebenes[driveItem](driveitem.md)-Objekt verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="346b0-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="346b0-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="346b0-106">JSON representation</span></span>

<span data-ttu-id="346b0-107">Es folgt eine JSON-Darstellung einer **sharedDriveItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="346b0-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="346b0-108">Die **sharedDriveItem**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="346b0-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="346b0-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="346b0-109">Properties</span></span>

| <span data-ttu-id="346b0-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="346b0-110">Property</span></span> | <span data-ttu-id="346b0-111">Typ</span><span class="sxs-lookup"><span data-stu-id="346b0-111">Type</span></span>                          | <span data-ttu-id="346b0-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="346b0-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="346b0-113">id</span><span class="sxs-lookup"><span data-stu-id="346b0-113">id</span></span>       | <span data-ttu-id="346b0-114">String</span><span class="sxs-lookup"><span data-stu-id="346b0-114">String</span></span>                        | <span data-ttu-id="346b0-115">Die eindeutige ID der Freigabe, auf die zugegriffen wird.</span><span class="sxs-lookup"><span data-stu-id="346b0-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="346b0-116">name</span><span class="sxs-lookup"><span data-stu-id="346b0-116">name</span></span>     | <span data-ttu-id="346b0-117">String</span><span class="sxs-lookup"><span data-stu-id="346b0-117">String</span></span>                        | <span data-ttu-id="346b0-118">Der Anzeigename für das freigegebene Element.</span><span class="sxs-lookup"><span data-stu-id="346b0-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="346b0-119">owner</span><span class="sxs-lookup"><span data-stu-id="346b0-119">owner</span></span>    | [<span data-ttu-id="346b0-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="346b0-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="346b0-121">Informationen zum Besitzer des freigegebenen Elements, auf das verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="346b0-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="346b0-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="346b0-122">Relationships</span></span>

| <span data-ttu-id="346b0-123">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="346b0-123">Relationship name</span></span> | <span data-ttu-id="346b0-124">Typ</span><span class="sxs-lookup"><span data-stu-id="346b0-124">Type</span></span>                | <span data-ttu-id="346b0-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="346b0-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="346b0-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="346b0-126">**driveItem**</span></span>     | <span data-ttu-id="346b0-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="346b0-127">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="346b0-128">Dient für den Zugriff auf das zugrunde liegende **driveItem**</span><span class="sxs-lookup"><span data-stu-id="346b0-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="346b0-129">**list**</span><span class="sxs-lookup"><span data-stu-id="346b0-129">**list**</span></span>          | <span data-ttu-id="346b0-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="346b0-130">[**list**][list]</span></span>           | <span data-ttu-id="346b0-131">Dient für den Zugriff auf das zugrunde liegende **list**</span><span class="sxs-lookup"><span data-stu-id="346b0-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="346b0-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="346b0-132">**listItem**</span></span>      | <span data-ttu-id="346b0-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="346b0-133">[**listItem**][listItem]</span></span>   | <span data-ttu-id="346b0-134">Dient für den Zugriff auf das zugrunde liegende **listItem**</span><span class="sxs-lookup"><span data-stu-id="346b0-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="346b0-135">**permission**</span><span class="sxs-lookup"><span data-stu-id="346b0-135">**permission**</span></span>    | <span data-ttu-id="346b0-136">[**Berechtigung**][permission]</span><span class="sxs-lookup"><span data-stu-id="346b0-136">[**permission**][permission]</span></span> | <span data-ttu-id="346b0-137">Verwendet, um die **Berechtigung** für den zugrunde liegenden sharing Hyperlink zugreifen</span><span class="sxs-lookup"><span data-stu-id="346b0-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="346b0-138">**site**</span><span class="sxs-lookup"><span data-stu-id="346b0-138">**site**</span></span>          | <span data-ttu-id="346b0-139">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="346b0-139">[**site**][site]</span></span>           | <span data-ttu-id="346b0-140">Dient für den Zugriff auf das zugrunde liegende **site**</span><span class="sxs-lookup"><span data-stu-id="346b0-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="346b0-141">Für in persönlichen OneDrive-Konten freigegebene **driveItems** könnenSie alternativ ebenfalls folgende Beziehungen verwenden.</span><span class="sxs-lookup"><span data-stu-id="346b0-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="346b0-142">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="346b0-142">Relationship name</span></span> | <span data-ttu-id="346b0-143">Typ</span><span class="sxs-lookup"><span data-stu-id="346b0-143">Type</span></span>                         | <span data-ttu-id="346b0-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="346b0-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="346b0-145">**items**</span><span class="sxs-lookup"><span data-stu-id="346b0-145">**items**</span></span>         | <span data-ttu-id="346b0-146">[**driveItem**][driveItem]-Sammmlung</span><span class="sxs-lookup"><span data-stu-id="346b0-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="346b0-147">Alle im Freigabestamm enthaltenen driveItems.</span><span class="sxs-lookup"><span data-stu-id="346b0-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="346b0-148">Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="346b0-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="346b0-149">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="346b0-149">**driveItem**</span></span>     | <span data-ttu-id="346b0-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="346b0-150">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="346b0-151">Dient für den Zugriff auf das zugrunde liegende **driveItem**</span><span class="sxs-lookup"><span data-stu-id="346b0-151">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="346b0-152">Methoden</span><span class="sxs-lookup"><span data-stu-id="346b0-152">Methods</span></span>

| <span data-ttu-id="346b0-153">Methode</span><span class="sxs-lookup"><span data-stu-id="346b0-153">Method</span></span>                                  | <span data-ttu-id="346b0-154">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="346b0-154">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="346b0-155">Freigegebenes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="346b0-155">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="346b0-156">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="346b0-156">Remarks</span></span>

<span data-ttu-id="346b0-157">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="346b0-157">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
