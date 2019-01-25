---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: f2493263d5293b95cbe386b46c56429d11dda089
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525087"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="d9cf6-102">Ressourcentyp incompleteData</span><span class="sxs-lookup"><span data-stu-id="d9cf6-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9cf6-103">Die **IncompleteData** Facetten gibt an, dass eine Ressource mit unvollständiger Daten generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="d9cf6-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="d9cf6-104">Die Eigenschaften innerhalb können Informationen über bereitzustellen, Grund, warum es unvollständige Daten.</span><span class="sxs-lookup"><span data-stu-id="d9cf6-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9cf6-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d9cf6-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="d9cf6-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d9cf6-106">Properties</span></span>

| <span data-ttu-id="d9cf6-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d9cf6-107">Property</span></span>                  | <span data-ttu-id="d9cf6-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d9cf6-108">Type</span></span>           | <span data-ttu-id="d9cf6-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9cf6-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="d9cf6-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="d9cf6-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="d9cf6-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9cf6-111">DateTimeOffset</span></span> | <span data-ttu-id="d9cf6-112">Der Dienst hat keine Quelldaten vor dem angegebenen Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="d9cf6-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="d9cf6-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="d9cf6-113">wasThrottled</span></span>              | <span data-ttu-id="d9cf6-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9cf6-114">Boolean</span></span>        | <span data-ttu-id="d9cf6-115">Einige Daten wurde nicht übermäßig viele Aktivitäten aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="d9cf6-115">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": [
    "Error: /api-reference/beta/resources/incompletedata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
