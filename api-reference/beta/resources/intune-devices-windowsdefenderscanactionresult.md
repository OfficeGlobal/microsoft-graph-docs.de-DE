---
title: windowsDefenderScanActionResult-Ressourcentyp
description: Letzte Analyseergebnisse von Windows Defender
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 094880247ee2612d0066bb44aa6f6bb581f7efe5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148643"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="78ce3-103">windowsDefenderScanActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="78ce3-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="78ce3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78ce3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78ce3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="78ce3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78ce3-106">Letzte Analyseergebnisse von Windows Defender</span><span class="sxs-lookup"><span data-stu-id="78ce3-106">Windows Defender last scan result</span></span>


<span data-ttu-id="78ce3-107">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="78ce3-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="78ce3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78ce3-108">Properties</span></span>
|<span data-ttu-id="78ce3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78ce3-109">Property</span></span>|<span data-ttu-id="78ce3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="78ce3-110">Type</span></span>|<span data-ttu-id="78ce3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78ce3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78ce3-112">actionName</span><span class="sxs-lookup"><span data-stu-id="78ce3-112">actionName</span></span>|<span data-ttu-id="78ce3-113">String</span><span class="sxs-lookup"><span data-stu-id="78ce3-113">String</span></span>|<span data-ttu-id="78ce3-114">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="78ce3-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="78ce3-115">actionState</span><span class="sxs-lookup"><span data-stu-id="78ce3-115">actionState</span></span>|[<span data-ttu-id="78ce3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="78ce3-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="78ce3-117">Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="78ce3-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="78ce3-118">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="78ce3-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="78ce3-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="78ce3-119">startDateTime</span></span>|<span data-ttu-id="78ce3-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78ce3-120">DateTimeOffset</span></span>|<span data-ttu-id="78ce3-121">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="78ce3-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="78ce3-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="78ce3-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="78ce3-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78ce3-123">DateTimeOffset</span></span>|<span data-ttu-id="78ce3-124">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="78ce3-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="78ce3-125">scanType</span><span class="sxs-lookup"><span data-stu-id="78ce3-125">scanType</span></span>|<span data-ttu-id="78ce3-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78ce3-126">String</span></span>|<span data-ttu-id="78ce3-127">Überprüfungstyp, entweder vollständige oder schnelle Überprüfung</span><span class="sxs-lookup"><span data-stu-id="78ce3-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="78ce3-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="78ce3-128">Relationships</span></span>
<span data-ttu-id="78ce3-129">Keine</span><span class="sxs-lookup"><span data-stu-id="78ce3-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78ce3-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="78ce3-130">JSON Representation</span></span>
<span data-ttu-id="78ce3-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="78ce3-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```




