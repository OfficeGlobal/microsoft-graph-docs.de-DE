---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: 8c442ad8ff3b23d20e8377a224a3f67b00163f5f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820965"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="7f2bf-102">AsyncJobStatus-Ressource</span><span class="sxs-lookup"><span data-stu-id="7f2bf-102">AsyncJobStatus resource</span></span>

> <span data-ttu-id="7f2bf-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7f2bf-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f2bf-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7f2bf-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f2bf-105">Diese Ressource enthält Informationen zum Status des Fortschritts eines asynchronen Auftrags.</span><span class="sxs-lookup"><span data-stu-id="7f2bf-105">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="7f2bf-106">Die folgende API ruft die Rückgabe von **AsyncJobStatus**-Ressourcen auf:</span><span class="sxs-lookup"><span data-stu-id="7f2bf-106">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="7f2bf-107">Copy Item</span><span class="sxs-lookup"><span data-stu-id="7f2bf-107">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="7f2bf-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7f2bf-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="7f2bf-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7f2bf-109">Properties</span></span>

| <span data-ttu-id="7f2bf-110">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="7f2bf-110">Property name</span></span>          | <span data-ttu-id="7f2bf-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7f2bf-111">Type</span></span>   | <span data-ttu-id="7f2bf-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f2bf-112">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="7f2bf-113">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="7f2bf-113">**percentageComplete**</span></span> | <span data-ttu-id="7f2bf-114">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="7f2bf-114">Double</span></span> | <span data-ttu-id="7f2bf-115">Ein Wert zwischen 0 und 100, der den Prozentsatz der Fertigstellung angibt.</span><span class="sxs-lookup"><span data-stu-id="7f2bf-115">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="7f2bf-116">**status**</span><span class="sxs-lookup"><span data-stu-id="7f2bf-116">**status**</span></span>             | <span data-ttu-id="7f2bf-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f2bf-117">String</span></span> | <span data-ttu-id="7f2bf-118">Ein Zeichenfolgenwert, der eine Enumeration der möglichen Werte über den Status des Auftrags zuordnet.</span><span class="sxs-lookup"><span data-stu-id="7f2bf-118">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation"
} -->
