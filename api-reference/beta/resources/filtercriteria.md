---
title: FilterCriteria-Ressourcentyp
description: Stellt die auf eine Spalte angewendeten Filterkriterien dar.
ms.openlocfilehash: dbcc57ff940fec525b712eb11ac44209f5f8a4d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058838"
---
# <a name="filtercriteria-resource-type"></a><span data-ttu-id="76d31-103">FilterCriteria-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="76d31-103">FilterCriteria resource type</span></span>

> <span data-ttu-id="76d31-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="76d31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76d31-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="76d31-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76d31-106">Stellt die auf eine Spalte angewendeten Filterkriterien dar.</span><span class="sxs-lookup"><span data-stu-id="76d31-106">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76d31-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="76d31-107">JSON representation</span></span>

<span data-ttu-id="76d31-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="76d31-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": "string"
}

```