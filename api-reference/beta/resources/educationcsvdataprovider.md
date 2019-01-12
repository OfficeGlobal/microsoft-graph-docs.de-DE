---
title: Ressourcentyp educationCsvDataProvider
description: 'Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19ef77671f862a0b59b5697b76bb54dc20e42856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952755"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="40710-103">Ressourcentyp educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="40710-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="40710-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="40710-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40710-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40710-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40710-106">Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.</span><span class="sxs-lookup"><span data-stu-id="40710-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="40710-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="40710-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="40710-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="40710-108">Properties</span></span>

| <span data-ttu-id="40710-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40710-109">Property</span></span> | <span data-ttu-id="40710-110">Typ</span><span class="sxs-lookup"><span data-stu-id="40710-110">Type</span></span> | <span data-ttu-id="40710-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40710-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="40710-112">**Anpassungen**</span><span class="sxs-lookup"><span data-stu-id="40710-112">**customizations**</span></span> | [<span data-ttu-id="40710-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="40710-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="40710-114">Optional Anpassungen Synchronisierung Profil angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="40710-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40710-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="40710-115">JSON representation</span></span>

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
