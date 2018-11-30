---
title: Ressourcentyp educationCsvDataProvider
description: 'Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.  '
ms.openlocfilehash: a3079b4f18c74c95fb0f8646116f2c7901d17b3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058530"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="3b218-103">Ressourcentyp educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="3b218-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="3b218-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b218-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b218-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b218-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b218-106">Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.</span><span class="sxs-lookup"><span data-stu-id="3b218-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="3b218-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="3b218-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3b218-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3b218-108">Properties</span></span>

| <span data-ttu-id="3b218-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b218-109">Property</span></span> | <span data-ttu-id="3b218-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3b218-110">Type</span></span> | <span data-ttu-id="3b218-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b218-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="3b218-112">**Anpassungen**</span><span class="sxs-lookup"><span data-stu-id="3b218-112">**customizations**</span></span> | [<span data-ttu-id="3b218-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="3b218-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="3b218-114">Optional Anpassungen Synchronisierung Profil angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3b218-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b218-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3b218-115">JSON representation</span></span>

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
