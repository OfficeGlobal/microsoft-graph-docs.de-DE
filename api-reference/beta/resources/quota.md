---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Kontingent
localization_priority: Normal
ms.openlocfilehash: a63b41253569dbb3d666a76b0a7495839ef61b12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882411"
---
# <a name="quota-resource-type"></a><span data-ttu-id="d08ca-102">Kontingent Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d08ca-102">quota resource type</span></span>

> <span data-ttu-id="d08ca-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d08ca-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d08ca-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d08ca-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d08ca-105">Die Ressource **Kontingent** enthält Details zu verwendeten Speicherplatz für eine Ressource [Laufwerk](drive.md) schränkt.</span><span class="sxs-lookup"><span data-stu-id="d08ca-105">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d08ca-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d08ca-106">JSON representation</span></span>

<span data-ttu-id="d08ca-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d08ca-107">Here is a JSON representation of the resource.</span></span>

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
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="d08ca-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d08ca-108">Properties</span></span>

| <span data-ttu-id="d08ca-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="d08ca-109">Property name</span></span> | <span data-ttu-id="d08ca-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d08ca-110">Type</span></span>   | <span data-ttu-id="d08ca-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d08ca-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="d08ca-112">gesamt</span><span class="sxs-lookup"><span data-stu-id="d08ca-112">total</span></span>         | <span data-ttu-id="d08ca-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d08ca-113">Int64</span></span>  | <span data-ttu-id="d08ca-p102">Zulässige Speicherplatz in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d08ca-p102">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="d08ca-116">verwendet</span><span class="sxs-lookup"><span data-stu-id="d08ca-116">used</span></span>          | <span data-ttu-id="d08ca-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d08ca-117">Int64</span></span>  | <span data-ttu-id="d08ca-p103">Gesamter verwendeter Speicherplatz in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d08ca-p103">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="d08ca-120">verbleibende</span><span class="sxs-lookup"><span data-stu-id="d08ca-120">remaining</span></span>     | <span data-ttu-id="d08ca-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d08ca-121">Int64</span></span>  | <span data-ttu-id="d08ca-p104">Gesamter verbleibender Speicherplatz vor dem Erreichen des Speicherkontingents in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d08ca-p104">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="d08ca-124">gelöscht</span><span class="sxs-lookup"><span data-stu-id="d08ca-124">deleted</span></span>       | <span data-ttu-id="d08ca-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d08ca-125">Int64</span></span>  | <span data-ttu-id="d08ca-p105">Gesamte Dateien genutzter Speicherplatz im Papierkorb in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d08ca-p105">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="d08ca-128">state</span><span class="sxs-lookup"><span data-stu-id="d08ca-128">state</span></span>         | <span data-ttu-id="d08ca-129">string</span><span class="sxs-lookup"><span data-stu-id="d08ca-129">string</span></span> | <span data-ttu-id="d08ca-p106">Wert der Enumeration, die den Zustand des Speicherplatzes angibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d08ca-p106">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="d08ca-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="d08ca-132">storagePlanInformation</span></span>  | [<span data-ttu-id="d08ca-133">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="d08ca-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="d08ca-134">Informationen über das Laufwerk Speicherung Kontingent Pläne.</span><span class="sxs-lookup"><span data-stu-id="d08ca-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="d08ca-135">Nur in der persönlichen OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d08ca-135">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="d08ca-136">State Enumerationswerte</span><span class="sxs-lookup"><span data-stu-id="d08ca-136">State enumeration values</span></span>

| <span data-ttu-id="d08ca-137">Wert</span><span class="sxs-lookup"><span data-stu-id="d08ca-137">Value</span></span>      | <span data-ttu-id="d08ca-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d08ca-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="d08ca-139">Das Laufwerk verfügt über ausreichend verbleibendes Kontingent.</span><span class="sxs-lookup"><span data-stu-id="d08ca-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="d08ca-140">Verbleibendes Kontingent weniger als 10 % des gesamten Kontingentplatzes.</span><span class="sxs-lookup"><span data-stu-id="d08ca-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="d08ca-141">Verbleibendes Kontingent weniger als 1 % des gesamten Kontingentplatzes.</span><span class="sxs-lookup"><span data-stu-id="d08ca-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="d08ca-p108">Das verwendete Kontingent hat das gesamte Kontingent überschritten. Neue Dateien oder Ordner können nicht hinzugefügt werden, wenn sie nicht unter dem Betrag für das Gesamtkontingent liegen oder mehr Speicherplatz erworben wird.</span><span class="sxs-lookup"><span data-stu-id="d08ca-p108">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota"
} -->
