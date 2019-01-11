---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Kontingent
localization_priority: Normal
ms.openlocfilehash: 58969adb525736b8a665844a5fa4b48ae4ca1831
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848412"
---
# <a name="quota-resource-type"></a><span data-ttu-id="556aa-102">Quota-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="556aa-102">Quota resource type</span></span>

<span data-ttu-id="556aa-103">Die **quota**-Ressource enthält Details zu Leerzeichenbeschränkungen auf einer[Laufwerk](drive.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="556aa-103">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="556aa-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="556aa-104">JSON representation</span></span>

<span data-ttu-id="556aa-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="556aa-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="556aa-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="556aa-106">Properties</span></span>

| <span data-ttu-id="556aa-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="556aa-107">Property name</span></span> | <span data-ttu-id="556aa-108">Typ</span><span class="sxs-lookup"><span data-stu-id="556aa-108">Type</span></span>   | <span data-ttu-id="556aa-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="556aa-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="556aa-110">gesamt</span><span class="sxs-lookup"><span data-stu-id="556aa-110">total</span></span>         | <span data-ttu-id="556aa-111">Int64</span><span class="sxs-lookup"><span data-stu-id="556aa-111">Int64</span></span>  | <span data-ttu-id="556aa-p101">Zulässige Speicherplatz in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="556aa-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="556aa-114">verwendet</span><span class="sxs-lookup"><span data-stu-id="556aa-114">used</span></span>          | <span data-ttu-id="556aa-115">Int64</span><span class="sxs-lookup"><span data-stu-id="556aa-115">Int64</span></span>  | <span data-ttu-id="556aa-p102">Gesamter verwendeter Speicherplatz in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="556aa-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="556aa-118">verbleibende</span><span class="sxs-lookup"><span data-stu-id="556aa-118">remaining</span></span>     | <span data-ttu-id="556aa-119">Int64</span><span class="sxs-lookup"><span data-stu-id="556aa-119">Int64</span></span>  | <span data-ttu-id="556aa-p103">Gesamter verbleibender Speicherplatz vor dem Erreichen des Speicherkontingents in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="556aa-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="556aa-122">gelöscht</span><span class="sxs-lookup"><span data-stu-id="556aa-122">deleted</span></span>       | <span data-ttu-id="556aa-123">Int64</span><span class="sxs-lookup"><span data-stu-id="556aa-123">Int64</span></span>  | <span data-ttu-id="556aa-p104">Gesamte Dateien genutzter Speicherplatz im Papierkorb in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="556aa-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="556aa-126">state</span><span class="sxs-lookup"><span data-stu-id="556aa-126">state</span></span>         | <span data-ttu-id="556aa-127">string</span><span class="sxs-lookup"><span data-stu-id="556aa-127">string</span></span> | <span data-ttu-id="556aa-p105">Wert der Enumeration, die den Zustand des Speicherplatzes angibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="556aa-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="556aa-130">Status Enumeration</span><span class="sxs-lookup"><span data-stu-id="556aa-130">State Enumeration</span></span>

| <span data-ttu-id="556aa-131">Wert</span><span class="sxs-lookup"><span data-stu-id="556aa-131">Value</span></span>      | <span data-ttu-id="556aa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="556aa-132">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="556aa-133">Das Laufwerk verfügt über ausreichend verbleibendes Kontingent.</span><span class="sxs-lookup"><span data-stu-id="556aa-133">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="556aa-134">Verbleibendes Kontingent weniger als 10 % des gesamten Kontingentplatzes.</span><span class="sxs-lookup"><span data-stu-id="556aa-134">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="556aa-135">Verbleibendes Kontingent weniger als 1 % des gesamten Kontingentplatzes.</span><span class="sxs-lookup"><span data-stu-id="556aa-135">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="556aa-p106">Das verwendete Kontingent hat das gesamte Kontingent überschritten. Neue Dateien oder Ordner können nicht hinzugefügt werden, wenn sie nicht unter dem Betrag für das Gesamtkontingent liegen oder mehr Speicherplatz erworben wird.</span><span class="sxs-lookup"><span data-stu-id="556aa-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/quota.md:
      Found potential enums in resource example that weren't defined in a table:(normal, nearing,critical,exceeded) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Quota"
} -->
