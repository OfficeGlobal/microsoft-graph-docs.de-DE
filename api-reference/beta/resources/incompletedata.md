---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: add1e3612f65e203f2437419cbb105b78025aa0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807511"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="3a212-102">Ressourcentyp incompleteData</span><span class="sxs-lookup"><span data-stu-id="3a212-102">incompleteData resource type</span></span>

 > <span data-ttu-id="3a212-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3a212-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a212-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3a212-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a212-105">Die **IncompleteData** Facetten gibt an, dass eine Ressource mit unvollständiger Daten generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="3a212-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="3a212-106">Die Eigenschaften innerhalb können Informationen über bereitzustellen, Grund, warum es unvollständige Daten.</span><span class="sxs-lookup"><span data-stu-id="3a212-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a212-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3a212-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="3a212-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3a212-108">Properties</span></span>

| <span data-ttu-id="3a212-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3a212-109">Property</span></span>                  | <span data-ttu-id="3a212-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3a212-110">Type</span></span>           | <span data-ttu-id="3a212-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a212-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="3a212-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="3a212-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="3a212-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a212-113">DateTimeOffset</span></span> | <span data-ttu-id="3a212-114">Der Dienst hat keine Quelldaten vor dem angegebenen Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="3a212-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="3a212-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="3a212-115">wasThrottled</span></span>              | <span data-ttu-id="3a212-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3a212-116">Boolean</span></span>        | <span data-ttu-id="3a212-117">Einige Daten wurde nicht übermäßig viele Aktivitäten aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="3a212-117">Some data was not recorded due to excessive activity.</span></span>

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
