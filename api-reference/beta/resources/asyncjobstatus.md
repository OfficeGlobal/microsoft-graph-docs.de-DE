---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
ms.openlocfilehash: 9e0f95802f9f75930384ab1534bf4c519fd9cfeb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058474"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="9625b-102">AsyncJobStatus-Ressource</span><span class="sxs-lookup"><span data-stu-id="9625b-102">AsyncJobStatus resource</span></span>

> <span data-ttu-id="9625b-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9625b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9625b-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9625b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9625b-105">Diese Ressource enthält Informationen zum Status des Fortschritts eines asynchronen Auftrags.</span><span class="sxs-lookup"><span data-stu-id="9625b-105">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="9625b-106">Die folgende API ruft die Rückgabe von **AsyncJobStatus**-Ressourcen auf:</span><span class="sxs-lookup"><span data-stu-id="9625b-106">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="9625b-107">Copy Item</span><span class="sxs-lookup"><span data-stu-id="9625b-107">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="9625b-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9625b-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="9625b-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9625b-109">Properties</span></span>

| <span data-ttu-id="9625b-110">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="9625b-110">Property name</span></span>          | <span data-ttu-id="9625b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="9625b-111">Type</span></span>   | <span data-ttu-id="9625b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9625b-112">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="9625b-113">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="9625b-113">**percentageComplete**</span></span> | <span data-ttu-id="9625b-114">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="9625b-114">Double</span></span> | <span data-ttu-id="9625b-115">Ein Wert zwischen 0 und 100, der den Prozentsatz der Fertigstellung angibt.</span><span class="sxs-lookup"><span data-stu-id="9625b-115">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="9625b-116">**status**</span><span class="sxs-lookup"><span data-stu-id="9625b-116">**status**</span></span>             | <span data-ttu-id="9625b-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9625b-117">String</span></span> | <span data-ttu-id="9625b-118">Ein Zeichenfolgenwert, der eine Enumeration der möglichen Werte über den Status des Auftrags zuordnet.</span><span class="sxs-lookup"><span data-stu-id="9625b-118">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation"
} -->
