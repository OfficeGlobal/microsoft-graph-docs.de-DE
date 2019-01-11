---
title: Ressourcentyp convertIdResult
description: Das Ergebnis einer ID formatkonvertierung, die von der Funktion TranslateExchangeIds durchgeführt.
localization_priority: Normal
ms.openlocfilehash: 7e1878de3d3b7ddee36d799c928d6a130b578200
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821455"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="32677-103">Ressourcentyp convertIdResult</span><span class="sxs-lookup"><span data-stu-id="32677-103">convertIdResult resource type</span></span>

> <span data-ttu-id="32677-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="32677-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32677-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="32677-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32677-106">Das Ergebnis einer ID formatkonvertierung, die von der Funktion [TranslateExchangeIds](../api/user-translateexchangeids.md) durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="32677-106">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="32677-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="32677-107">Properties</span></span>

| <span data-ttu-id="32677-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32677-108">Property</span></span> | <span data-ttu-id="32677-109">Typ</span><span class="sxs-lookup"><span data-stu-id="32677-109">Type</span></span> | <span data-ttu-id="32677-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32677-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="32677-111">sourceId</span><span class="sxs-lookup"><span data-stu-id="32677-111">sourceId</span></span> | <span data-ttu-id="32677-112">String</span><span class="sxs-lookup"><span data-stu-id="32677-112">String</span></span> | <span data-ttu-id="32677-113">Der Bezeichner, der konvertiert wurde.</span><span class="sxs-lookup"><span data-stu-id="32677-113">The identifier that was converted.</span></span> <span data-ttu-id="32677-114">Dieser Wert ist der ursprüngliche, nicht konvertierten Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="32677-114">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="32677-115">targetId</span><span class="sxs-lookup"><span data-stu-id="32677-115">targetId</span></span> | <span data-ttu-id="32677-116">String</span><span class="sxs-lookup"><span data-stu-id="32677-116">String</span></span> | <span data-ttu-id="32677-117">Der Bezeichner konvertierte.</span><span class="sxs-lookup"><span data-stu-id="32677-117">The converted identifier.</span></span> <span data-ttu-id="32677-118">Dieser Wert ist nicht vorhanden, wenn die Konvertierung fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="32677-118">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="32677-119">errorDetails</span><span class="sxs-lookup"><span data-stu-id="32677-119">errorDetails</span></span> | [<span data-ttu-id="32677-120">Allgemeiner Fehler</span><span class="sxs-lookup"><span data-stu-id="32677-120">genericError</span></span>](genericerror.md) | <span data-ttu-id="32677-121">Ein Error-Objekt zurück, der den Grund für die Konvertierungsfehler angibt.</span><span class="sxs-lookup"><span data-stu-id="32677-121">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="32677-122">Dieser Wert ist nicht vorhanden, wenn die Konvertierung erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="32677-122">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="32677-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="32677-123">JSON representation</span></span>

<span data-ttu-id="32677-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="32677-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
