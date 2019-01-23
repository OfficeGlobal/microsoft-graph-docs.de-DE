---
title: Ressourcentyp educationCsvDataProvider
description: 'Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c9211d5f7ca25b78c6e76c3744f6941e3b172bb3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399346"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="f8aca-103">Ressourcentyp educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="f8aca-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="f8aca-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="f8aca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8aca-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8aca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8aca-106">Verwendet, um die Synchronisierung Schule Datenprofil beim CSV-Dateien die Eingabe Quelle sind einzurichten.</span><span class="sxs-lookup"><span data-stu-id="f8aca-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="f8aca-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="f8aca-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f8aca-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8aca-108">Properties</span></span>

| <span data-ttu-id="f8aca-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8aca-109">Property</span></span> | <span data-ttu-id="f8aca-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f8aca-110">Type</span></span> | <span data-ttu-id="f8aca-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8aca-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f8aca-112">**Anpassungen**</span><span class="sxs-lookup"><span data-stu-id="f8aca-112">**customizations**</span></span> | [<span data-ttu-id="f8aca-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="f8aca-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="f8aca-114">Optional Anpassungen Synchronisierung Profil angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f8aca-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8aca-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8aca-115">JSON representation</span></span>

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
