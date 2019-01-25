---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Kontingent
localization_priority: Normal
ms.openlocfilehash: ce07852592317568254217c7e869f1da7f296a2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525486"
---
# <a name="quota-resource-type"></a><span data-ttu-id="873a1-102">Quota-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="873a1-102">quota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="873a1-103">Die **quota**-Ressource enthält Details zu Leerzeichenbeschränkungen auf einer[Laufwerk](drive.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="873a1-103">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="873a1-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="873a1-104">JSON representation</span></span>

<span data-ttu-id="873a1-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="873a1-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="873a1-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="873a1-106">Properties</span></span>

| <span data-ttu-id="873a1-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="873a1-107">Property name</span></span> | <span data-ttu-id="873a1-108">Typ</span><span class="sxs-lookup"><span data-stu-id="873a1-108">Type</span></span>   | <span data-ttu-id="873a1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="873a1-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="873a1-110">gesamt</span><span class="sxs-lookup"><span data-stu-id="873a1-110">total</span></span>         | <span data-ttu-id="873a1-111">Int64</span><span class="sxs-lookup"><span data-stu-id="873a1-111">Int64</span></span>  | <span data-ttu-id="873a1-p101">Zulässige Speicherplatz in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="873a1-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="873a1-114">verwendet</span><span class="sxs-lookup"><span data-stu-id="873a1-114">used</span></span>          | <span data-ttu-id="873a1-115">Int64</span><span class="sxs-lookup"><span data-stu-id="873a1-115">Int64</span></span>  | <span data-ttu-id="873a1-p102">Gesamter verwendeter Speicherplatz in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="873a1-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="873a1-118">verbleibende</span><span class="sxs-lookup"><span data-stu-id="873a1-118">remaining</span></span>     | <span data-ttu-id="873a1-119">Int64</span><span class="sxs-lookup"><span data-stu-id="873a1-119">Int64</span></span>  | <span data-ttu-id="873a1-p103">Gesamter verbleibender Speicherplatz vor dem Erreichen des Speicherkontingents in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="873a1-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="873a1-122">gelöscht</span><span class="sxs-lookup"><span data-stu-id="873a1-122">deleted</span></span>       | <span data-ttu-id="873a1-123">Int64</span><span class="sxs-lookup"><span data-stu-id="873a1-123">Int64</span></span>  | <span data-ttu-id="873a1-p104">Gesamte Dateien genutzter Speicherplatz im Papierkorb in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="873a1-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="873a1-126">state</span><span class="sxs-lookup"><span data-stu-id="873a1-126">state</span></span>         | <span data-ttu-id="873a1-127">string</span><span class="sxs-lookup"><span data-stu-id="873a1-127">string</span></span> | <span data-ttu-id="873a1-p105">Wert der Enumeration, die den Zustand des Speicherplatzes angibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="873a1-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="873a1-130">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="873a1-130">storagePlanInformation</span></span>  | [<span data-ttu-id="873a1-131">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="873a1-131">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="873a1-132">Informationen über das Laufwerk Speicherung Kontingent Pläne.</span><span class="sxs-lookup"><span data-stu-id="873a1-132">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="873a1-133">Nur in der persönlichen OneDrive.</span><span class="sxs-lookup"><span data-stu-id="873a1-133">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="873a1-134">State Enumerationswerte</span><span class="sxs-lookup"><span data-stu-id="873a1-134">State enumeration values</span></span>

| <span data-ttu-id="873a1-135">Wert</span><span class="sxs-lookup"><span data-stu-id="873a1-135">Value</span></span>      | <span data-ttu-id="873a1-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="873a1-136">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="873a1-137">Das Laufwerk verfügt über ausreichend verbleibendes Kontingent.</span><span class="sxs-lookup"><span data-stu-id="873a1-137">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="873a1-138">Verbleibendes Kontingent weniger als 10 % des gesamten Kontingentplatzes.</span><span class="sxs-lookup"><span data-stu-id="873a1-138">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="873a1-139">Verbleibendes Kontingent weniger als 1 % des gesamten Kontingentplatzes.</span><span class="sxs-lookup"><span data-stu-id="873a1-139">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="873a1-p107">Das verwendete Kontingent hat das gesamte Kontingent überschritten. Neue Dateien oder Ordner können nicht hinzugefügt werden, wenn sie nicht unter dem Betrag für das Gesamtkontingent liegen oder mehr Speicherplatz erworben wird.</span><span class="sxs-lookup"><span data-stu-id="873a1-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": [
    "Error: /api-reference/beta/resources/quota.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
