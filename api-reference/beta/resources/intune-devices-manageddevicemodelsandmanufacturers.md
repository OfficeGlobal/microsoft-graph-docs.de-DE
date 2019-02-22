---
title: managedDeviceModelsAndManufacturers-Ressourcentyp
description: Modelliert und fertigt meatadata für verwaltete Geräte im Konto
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfd8f068305bdae86a0acc9ef5f9113bb0d1c579
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148300"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="d5183-103">managedDeviceModelsAndManufacturers-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d5183-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="d5183-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5183-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5183-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d5183-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5183-106">Modelliert und fertigt meatadata für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="d5183-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="d5183-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d5183-107">Properties</span></span>
|<span data-ttu-id="d5183-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d5183-108">Property</span></span>|<span data-ttu-id="d5183-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d5183-109">Type</span></span>|<span data-ttu-id="d5183-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5183-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5183-111">deviceModels</span><span class="sxs-lookup"><span data-stu-id="d5183-111">deviceModels</span></span>|<span data-ttu-id="d5183-112">String collection</span><span class="sxs-lookup"><span data-stu-id="d5183-112">String collection</span></span>|<span data-ttu-id="d5183-113">Liste der Modelle für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="d5183-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="d5183-114">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="d5183-114">deviceManufacturers</span></span>|<span data-ttu-id="d5183-115">String collection</span><span class="sxs-lookup"><span data-stu-id="d5183-115">String collection</span></span>|<span data-ttu-id="d5183-116">Liste der Hersteller für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="d5183-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5183-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d5183-117">Relationships</span></span>
<span data-ttu-id="d5183-118">Keine</span><span class="sxs-lookup"><span data-stu-id="d5183-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5183-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d5183-119">JSON Representation</span></span>
<span data-ttu-id="d5183-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d5183-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```




