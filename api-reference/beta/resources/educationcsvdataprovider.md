---
title: Ressourcentyp educationCsvDataProvider
description: 'Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: cb4d08a2a6750310a825f66ecfb0017abacd36fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878569"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="85736-103">Ressourcentyp educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="85736-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="85736-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="85736-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85736-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85736-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85736-106">Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.</span><span class="sxs-lookup"><span data-stu-id="85736-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="85736-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="85736-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="85736-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85736-108">Properties</span></span>

| <span data-ttu-id="85736-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85736-109">Property</span></span> | <span data-ttu-id="85736-110">Typ</span><span class="sxs-lookup"><span data-stu-id="85736-110">Type</span></span> | <span data-ttu-id="85736-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85736-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="85736-112">**Anpassungen**</span><span class="sxs-lookup"><span data-stu-id="85736-112">**customizations**</span></span> | [<span data-ttu-id="85736-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="85736-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="85736-114">Optional Anpassungen Synchronisierung Profil angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="85736-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85736-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85736-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
