---
title: windowsDefenderScanActionResult-Ressourcentyp
description: Letzte Analyseergebnisse von Windows Defender
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20d30ebda6e24f26406d189ebd980e558bf74e83
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251342"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="77db5-103">windowsDefenderScanActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="77db5-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="77db5-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="77db5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77db5-105">Letzte Analyseergebnisse von Windows Defender</span><span class="sxs-lookup"><span data-stu-id="77db5-105">Windows Defender last scan result</span></span>


<span data-ttu-id="77db5-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="77db5-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="77db5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="77db5-107">Properties</span></span>
|<span data-ttu-id="77db5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77db5-108">Property</span></span>|<span data-ttu-id="77db5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="77db5-109">Type</span></span>|<span data-ttu-id="77db5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77db5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77db5-111">actionName</span><span class="sxs-lookup"><span data-stu-id="77db5-111">actionName</span></span>|<span data-ttu-id="77db5-112">String</span><span class="sxs-lookup"><span data-stu-id="77db5-112">String</span></span>|<span data-ttu-id="77db5-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="77db5-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="77db5-114">actionState</span><span class="sxs-lookup"><span data-stu-id="77db5-114">actionState</span></span>|[<span data-ttu-id="77db5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="77db5-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="77db5-116">Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="77db5-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="77db5-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="77db5-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="77db5-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="77db5-118">startDateTime</span></span>|<span data-ttu-id="77db5-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77db5-119">DateTimeOffset</span></span>|<span data-ttu-id="77db5-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="77db5-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="77db5-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="77db5-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="77db5-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77db5-122">DateTimeOffset</span></span>|<span data-ttu-id="77db5-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="77db5-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="77db5-124">scanType</span><span class="sxs-lookup"><span data-stu-id="77db5-124">scanType</span></span>|<span data-ttu-id="77db5-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77db5-125">String</span></span>|<span data-ttu-id="77db5-126">Überprüfungstyp, entweder vollständige oder schnelle Überprüfung</span><span class="sxs-lookup"><span data-stu-id="77db5-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="77db5-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="77db5-127">Relationships</span></span>
<span data-ttu-id="77db5-128">Keine</span><span class="sxs-lookup"><span data-stu-id="77db5-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77db5-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="77db5-129">JSON Representation</span></span>
<span data-ttu-id="77db5-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="77db5-130">Here is a JSON representation of the resource.</span></span>
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



