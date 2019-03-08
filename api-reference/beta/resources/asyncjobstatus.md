---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: c951aa05b2b0f6f2b036bdf145e161a8d5b52ba7
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482231"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="fea2c-102">AsyncJobStatus-Ressource</span><span class="sxs-lookup"><span data-stu-id="fea2c-102">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fea2c-103">Diese Ressource enthält Informationen zum Status des Fortschritts eines asynchronen Auftrags.</span><span class="sxs-lookup"><span data-stu-id="fea2c-103">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="fea2c-104">Die folgende API ruft die Rückgabe von **AsyncJobStatus**-Ressourcen auf:</span><span class="sxs-lookup"><span data-stu-id="fea2c-104">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="fea2c-105">Copy Item</span><span class="sxs-lookup"><span data-stu-id="fea2c-105">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="fea2c-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fea2c-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="fea2c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fea2c-107">Properties</span></span>

| <span data-ttu-id="fea2c-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="fea2c-108">Property name</span></span>          | <span data-ttu-id="fea2c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="fea2c-109">Type</span></span>   | <span data-ttu-id="fea2c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fea2c-110">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="fea2c-111">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="fea2c-111">**percentageComplete**</span></span> | <span data-ttu-id="fea2c-112">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="fea2c-112">Double</span></span> | <span data-ttu-id="fea2c-113">Ein Wert zwischen 0 und 100, der den Prozentsatz der Fertigstellung angibt.</span><span class="sxs-lookup"><span data-stu-id="fea2c-113">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="fea2c-114">**status**</span><span class="sxs-lookup"><span data-stu-id="fea2c-114">**status**</span></span>             | <span data-ttu-id="fea2c-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fea2c-115">String</span></span> | <span data-ttu-id="fea2c-116">Ein Zeichenfolgenwert, der eine Enumeration der möglichen Werte über den Status des Auftrags zuordnet.</span><span class="sxs-lookup"><span data-stu-id="fea2c-116">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/asyncjobstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
