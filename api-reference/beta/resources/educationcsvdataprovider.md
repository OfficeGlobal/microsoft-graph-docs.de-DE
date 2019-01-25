---
title: Ressourcentyp educationCsvDataProvider
description: 'Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bebacbc1c618c7558d81bde2611840e8d225a8fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529873"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="bd9fa-103">Ressourcentyp educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="bd9fa-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd9fa-104">Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.</span><span class="sxs-lookup"><span data-stu-id="bd9fa-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="bd9fa-105">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="bd9fa-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bd9fa-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd9fa-106">Properties</span></span>

| <span data-ttu-id="bd9fa-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd9fa-107">Property</span></span> | <span data-ttu-id="bd9fa-108">Typ</span><span class="sxs-lookup"><span data-stu-id="bd9fa-108">Type</span></span> | <span data-ttu-id="bd9fa-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd9fa-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="bd9fa-110">**Anpassungen**</span><span class="sxs-lookup"><span data-stu-id="bd9fa-110">**customizations**</span></span> | [<span data-ttu-id="bd9fa-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="bd9fa-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="bd9fa-112">Optional Anpassungen Synchronisierung Profil angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="bd9fa-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd9fa-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd9fa-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcsvdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
