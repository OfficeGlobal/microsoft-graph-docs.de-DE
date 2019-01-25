---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 22e449d725b94b7be458261e82cfde0b5d6fdf9c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524121"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="4f5fc-102">SharedDriveItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4f5fc-102">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f5fc-103">Die **sharedDriveItem**-Ressource wird zurückgegeben, wenn die [Freigabe](../api/shares-get.md)-API für den Zugriff auf ein freigegebenes[driveItem](driveitem.md)-Objekt verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="4f5fc-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f5fc-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4f5fc-104">JSON representation</span></span>

<span data-ttu-id="4f5fc-105">Es folgt eine JSON-Darstellung einer **sharedDriveItem**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="4f5fc-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="4f5fc-106">Die **sharedDriveItem**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="4f5fc-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4f5fc-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4f5fc-107">Properties</span></span>

| <span data-ttu-id="4f5fc-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4f5fc-108">Property</span></span> | <span data-ttu-id="4f5fc-109">Typ</span><span class="sxs-lookup"><span data-stu-id="4f5fc-109">Type</span></span>                          | <span data-ttu-id="4f5fc-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f5fc-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="4f5fc-111">id</span><span class="sxs-lookup"><span data-stu-id="4f5fc-111">id</span></span>       | <span data-ttu-id="4f5fc-112">String</span><span class="sxs-lookup"><span data-stu-id="4f5fc-112">String</span></span>                        | <span data-ttu-id="4f5fc-113">Die eindeutige ID der Freigabe, auf die zugegriffen wird.</span><span class="sxs-lookup"><span data-stu-id="4f5fc-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="4f5fc-114">name</span><span class="sxs-lookup"><span data-stu-id="4f5fc-114">name</span></span>     | <span data-ttu-id="4f5fc-115">String</span><span class="sxs-lookup"><span data-stu-id="4f5fc-115">String</span></span>                        | <span data-ttu-id="4f5fc-116">Der Anzeigename für das freigegebene Element.</span><span class="sxs-lookup"><span data-stu-id="4f5fc-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="4f5fc-117">owner</span><span class="sxs-lookup"><span data-stu-id="4f5fc-117">owner</span></span>    | [<span data-ttu-id="4f5fc-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="4f5fc-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="4f5fc-119">Informationen zum Besitzer des freigegebenen Elements, auf das verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="4f5fc-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4f5fc-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4f5fc-120">Relationships</span></span>

| <span data-ttu-id="4f5fc-121">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="4f5fc-121">Relationship name</span></span> | <span data-ttu-id="4f5fc-122">Typ</span><span class="sxs-lookup"><span data-stu-id="4f5fc-122">Type</span></span>                | <span data-ttu-id="4f5fc-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f5fc-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="4f5fc-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-124">**driveItem**</span></span>     | <span data-ttu-id="4f5fc-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="4f5fc-125">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="4f5fc-126">Dient für den Zugriff auf das zugrunde liegende **driveItem**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="4f5fc-127">**list**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-127">**list**</span></span>          | <span data-ttu-id="4f5fc-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="4f5fc-128">[**list**][list]</span></span>           | <span data-ttu-id="4f5fc-129">Dient für den Zugriff auf das zugrunde liegende **list**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="4f5fc-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-130">**listItem**</span></span>      | <span data-ttu-id="4f5fc-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="4f5fc-131">[**listItem**][listItem]</span></span>   | <span data-ttu-id="4f5fc-132">Dient für den Zugriff auf das zugrunde liegende **listItem**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="4f5fc-133">**permission**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-133">**permission**</span></span>    | <span data-ttu-id="4f5fc-134">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="4f5fc-134">[**permission**][permission]</span></span> | <span data-ttu-id="4f5fc-135">Verwendet, um die **Berechtigung** für den zugrunde liegenden sharing Hyperlink zugreifen</span><span class="sxs-lookup"><span data-stu-id="4f5fc-135">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="4f5fc-136">**site**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-136">**site**</span></span>          | <span data-ttu-id="4f5fc-137">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="4f5fc-137">[**site**][site]</span></span>           | <span data-ttu-id="4f5fc-138">Dient für den Zugriff auf das zugrunde liegende **site**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-138">Used to access the underlying **site**</span></span>

<span data-ttu-id="4f5fc-139">Für in persönlichen OneDrive-Konten freigegebene **driveItems** könnenSie alternativ ebenfalls folgende Beziehungen verwenden.</span><span class="sxs-lookup"><span data-stu-id="4f5fc-139">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="4f5fc-140">Beziehungsname</span><span class="sxs-lookup"><span data-stu-id="4f5fc-140">Relationship name</span></span> | <span data-ttu-id="4f5fc-141">Typ</span><span class="sxs-lookup"><span data-stu-id="4f5fc-141">Type</span></span>                         | <span data-ttu-id="4f5fc-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f5fc-142">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="4f5fc-143">**items**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-143">**items**</span></span>         | <span data-ttu-id="4f5fc-144">[**driveItem**][driveItem]-Sammmlung</span><span class="sxs-lookup"><span data-stu-id="4f5fc-144">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="4f5fc-145">Alle im Freigabestamm enthaltenen driveItems.</span><span class="sxs-lookup"><span data-stu-id="4f5fc-145">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="4f5fc-146">Diese Sammlung kann nicht aufgezählt werden.</span><span class="sxs-lookup"><span data-stu-id="4f5fc-146">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="4f5fc-147">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-147">**driveItem**</span></span>     | <span data-ttu-id="4f5fc-148">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="4f5fc-148">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="4f5fc-149">Dient für den Zugriff auf das zugrunde liegende **driveItem**</span><span class="sxs-lookup"><span data-stu-id="4f5fc-149">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="4f5fc-150">Methoden</span><span class="sxs-lookup"><span data-stu-id="4f5fc-150">Methods</span></span>

| <span data-ttu-id="4f5fc-151">Methode</span><span class="sxs-lookup"><span data-stu-id="4f5fc-151">Method</span></span>                                  | <span data-ttu-id="4f5fc-152">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="4f5fc-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="4f5fc-153">Freigegebenes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="4f5fc-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="4f5fc-154">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="4f5fc-154">Remarks</span></span>

<span data-ttu-id="4f5fc-155">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4f5fc-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": [
    "Error: /api-reference/beta/resources/shareddriveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
