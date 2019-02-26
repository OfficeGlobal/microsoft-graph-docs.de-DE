---
title: remoteLockActionResult-Ressourcentyp
description: Ergebnis einer Sperraktion mit einem Pin zum Entsperren
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c533d9590acba1518ac3d0dc791af804b9d84452
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260319"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="c8d31-103">remoteLockActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c8d31-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="c8d31-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c8d31-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8d31-105">Ergebnis einer Sperraktion mit einem Pin zum Entsperren</span><span class="sxs-lookup"><span data-stu-id="c8d31-105">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="c8d31-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c8d31-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8d31-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c8d31-107">Properties</span></span>
|<span data-ttu-id="c8d31-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c8d31-108">Property</span></span>|<span data-ttu-id="c8d31-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c8d31-109">Type</span></span>|<span data-ttu-id="c8d31-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8d31-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8d31-111">actionName</span><span class="sxs-lookup"><span data-stu-id="c8d31-111">actionName</span></span>|<span data-ttu-id="c8d31-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8d31-112">String</span></span>|<span data-ttu-id="c8d31-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c8d31-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c8d31-114">actionState</span><span class="sxs-lookup"><span data-stu-id="c8d31-114">actionState</span></span>|[<span data-ttu-id="c8d31-115">actionState</span><span class="sxs-lookup"><span data-stu-id="c8d31-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="c8d31-116">Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="c8d31-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c8d31-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c8d31-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c8d31-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c8d31-118">startDateTime</span></span>|<span data-ttu-id="c8d31-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8d31-119">DateTimeOffset</span></span>|<span data-ttu-id="c8d31-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c8d31-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c8d31-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8d31-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="c8d31-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8d31-122">DateTimeOffset</span></span>|<span data-ttu-id="c8d31-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c8d31-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c8d31-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="c8d31-124">unlockPin</span></span>|<span data-ttu-id="c8d31-125">String</span><span class="sxs-lookup"><span data-stu-id="c8d31-125">String</span></span>|<span data-ttu-id="c8d31-126">Pin zum Entsperren des Clients</span><span class="sxs-lookup"><span data-stu-id="c8d31-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8d31-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c8d31-127">Relationships</span></span>
<span data-ttu-id="c8d31-128">Keine</span><span class="sxs-lookup"><span data-stu-id="c8d31-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8d31-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c8d31-129">JSON Representation</span></span>
<span data-ttu-id="c8d31-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c8d31-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```



