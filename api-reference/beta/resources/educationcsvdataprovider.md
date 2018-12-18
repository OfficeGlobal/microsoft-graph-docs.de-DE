---
title: Ressourcentyp educationCsvDataProvider
description: 'Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.  '
author: mmast-msft
ms.openlocfilehash: 1a816d4e176147d549381465154e35cf0a821b98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317899"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="13b0f-103">Ressourcentyp educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="13b0f-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="13b0f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="13b0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13b0f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13b0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13b0f-106">Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.</span><span class="sxs-lookup"><span data-stu-id="13b0f-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="13b0f-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="13b0f-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="13b0f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13b0f-108">Properties</span></span>

| <span data-ttu-id="13b0f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13b0f-109">Property</span></span> | <span data-ttu-id="13b0f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="13b0f-110">Type</span></span> | <span data-ttu-id="13b0f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13b0f-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="13b0f-112">**Anpassungen**</span><span class="sxs-lookup"><span data-stu-id="13b0f-112">**customizations**</span></span> | [<span data-ttu-id="13b0f-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="13b0f-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="13b0f-114">Optional Anpassungen Synchronisierung Profil angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="13b0f-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13b0f-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13b0f-115">JSON representation</span></span>

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
