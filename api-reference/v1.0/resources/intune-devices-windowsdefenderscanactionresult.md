---
title: windowsDefenderScanActionResult-Ressourcentyp
description: Letzte Analyseergebnisse von Windows Defender
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 407db79fa0caf333dfb092620320aeb339e1b195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812152"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="bdac2-103">windowsDefenderScanActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bdac2-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="bdac2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bdac2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdac2-105">Letzte Analyseergebnisse von Windows Defender</span><span class="sxs-lookup"><span data-stu-id="bdac2-105">Windows Defender last scan result</span></span>

<span data-ttu-id="bdac2-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bdac2-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bdac2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bdac2-107">Properties</span></span>
|<span data-ttu-id="bdac2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bdac2-108">Property</span></span>|<span data-ttu-id="bdac2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bdac2-109">Type</span></span>|<span data-ttu-id="bdac2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdac2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdac2-111">actionName</span><span class="sxs-lookup"><span data-stu-id="bdac2-111">actionName</span></span>|<span data-ttu-id="bdac2-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdac2-112">String</span></span>|<span data-ttu-id="bdac2-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bdac2-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bdac2-114">actionState</span><span class="sxs-lookup"><span data-stu-id="bdac2-114">actionState</span></span>|[<span data-ttu-id="bdac2-115">actionState</span><span class="sxs-lookup"><span data-stu-id="bdac2-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="bdac2-116">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bdac2-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="bdac2-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bdac2-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bdac2-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bdac2-118">startDateTime</span></span>|<span data-ttu-id="bdac2-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdac2-119">DateTimeOffset</span></span>|<span data-ttu-id="bdac2-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bdac2-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bdac2-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdac2-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="bdac2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdac2-122">DateTimeOffset</span></span>|<span data-ttu-id="bdac2-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bdac2-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bdac2-124">scanType</span><span class="sxs-lookup"><span data-stu-id="bdac2-124">scanType</span></span>|<span data-ttu-id="bdac2-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdac2-125">String</span></span>|<span data-ttu-id="bdac2-126">Überprüfungstyp, entweder vollständige oder schnelle Überprüfung</span><span class="sxs-lookup"><span data-stu-id="bdac2-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdac2-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bdac2-127">Relationships</span></span>
<span data-ttu-id="bdac2-128">Keine</span><span class="sxs-lookup"><span data-stu-id="bdac2-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bdac2-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bdac2-129">JSON Representation</span></span>
<span data-ttu-id="bdac2-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bdac2-130">Here is a JSON representation of the resource.</span></span>
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



