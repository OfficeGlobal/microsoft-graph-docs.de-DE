---
title: remoteLockActionResult-Ressourcentyp
description: Ergebnis einer Sperraktion mit einem Pin zum Entsperren
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f90cbc46ca4bc9476ad5d9386581385ae7354261
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159024"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="86b8a-103">remoteLockActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="86b8a-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="86b8a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="86b8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86b8a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="86b8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86b8a-106">Ergebnis einer Sperraktion mit einem Pin zum Entsperren</span><span class="sxs-lookup"><span data-stu-id="86b8a-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="86b8a-107">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="86b8a-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="86b8a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="86b8a-108">Properties</span></span>
|<span data-ttu-id="86b8a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86b8a-109">Property</span></span>|<span data-ttu-id="86b8a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="86b8a-110">Type</span></span>|<span data-ttu-id="86b8a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86b8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86b8a-112">actionName</span><span class="sxs-lookup"><span data-stu-id="86b8a-112">actionName</span></span>|<span data-ttu-id="86b8a-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86b8a-113">String</span></span>|<span data-ttu-id="86b8a-114">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="86b8a-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="86b8a-115">actionState</span><span class="sxs-lookup"><span data-stu-id="86b8a-115">actionState</span></span>|[<span data-ttu-id="86b8a-116">actionState</span><span class="sxs-lookup"><span data-stu-id="86b8a-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="86b8a-117">Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="86b8a-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="86b8a-118">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="86b8a-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="86b8a-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="86b8a-119">startDateTime</span></span>|<span data-ttu-id="86b8a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86b8a-120">DateTimeOffset</span></span>|<span data-ttu-id="86b8a-121">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="86b8a-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="86b8a-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="86b8a-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="86b8a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86b8a-123">DateTimeOffset</span></span>|<span data-ttu-id="86b8a-124">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="86b8a-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="86b8a-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="86b8a-125">unlockPin</span></span>|<span data-ttu-id="86b8a-126">String</span><span class="sxs-lookup"><span data-stu-id="86b8a-126">String</span></span>|<span data-ttu-id="86b8a-127">Pin zum Entsperren des Clients</span><span class="sxs-lookup"><span data-stu-id="86b8a-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="86b8a-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="86b8a-128">Relationships</span></span>
<span data-ttu-id="86b8a-129">Keine</span><span class="sxs-lookup"><span data-stu-id="86b8a-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86b8a-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="86b8a-130">JSON Representation</span></span>
<span data-ttu-id="86b8a-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="86b8a-131">Here is a JSON representation of the resource.</span></span>
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




