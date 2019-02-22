---
title: deviceActionResult-Ressourcentyp
description: Ergebnis von Geräteaktion
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c435241056f5e29166355829d1c40438b525a92
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151429"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="a5e8a-103">deviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a5e8a-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="a5e8a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5e8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5e8a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a5e8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5e8a-106">Ergebnis von Gerätevorgang</span><span class="sxs-lookup"><span data-stu-id="a5e8a-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="a5e8a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a5e8a-107">Properties</span></span>
|<span data-ttu-id="a5e8a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5e8a-108">Property</span></span>|<span data-ttu-id="a5e8a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a5e8a-109">Type</span></span>|<span data-ttu-id="a5e8a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5e8a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5e8a-111">actionName</span><span class="sxs-lookup"><span data-stu-id="a5e8a-111">actionName</span></span>|<span data-ttu-id="a5e8a-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5e8a-112">String</span></span>|<span data-ttu-id="a5e8a-113">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="a5e8a-113">Action name</span></span>|
|<span data-ttu-id="a5e8a-114">actionState</span><span class="sxs-lookup"><span data-stu-id="a5e8a-114">actionState</span></span>|[<span data-ttu-id="a5e8a-115">actionState</span><span class="sxs-lookup"><span data-stu-id="a5e8a-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a5e8a-116">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="a5e8a-116">State of the action.</span></span> <span data-ttu-id="a5e8a-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a5e8a-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a5e8a-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a5e8a-118">startDateTime</span></span>|<span data-ttu-id="a5e8a-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5e8a-119">DateTimeOffset</span></span>|<span data-ttu-id="a5e8a-120">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="a5e8a-120">Time the action was initiated</span></span>|
|<span data-ttu-id="a5e8a-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5e8a-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="a5e8a-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5e8a-122">DateTimeOffset</span></span>|<span data-ttu-id="a5e8a-123">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="a5e8a-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5e8a-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a5e8a-124">Relationships</span></span>
<span data-ttu-id="a5e8a-125">Keine</span><span class="sxs-lookup"><span data-stu-id="a5e8a-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5e8a-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a5e8a-126">JSON Representation</span></span>
<span data-ttu-id="a5e8a-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a5e8a-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




