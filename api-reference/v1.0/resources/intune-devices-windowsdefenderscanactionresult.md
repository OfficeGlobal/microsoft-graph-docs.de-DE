---
title: windowsDefenderScanActionResult-Ressourcentyp
description: Letzte Analyseergebnisse von Windows Defender
ms.openlocfilehash: 6221e0d746e677f09b2be00ec66a898e6dfc288c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016397"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="29a89-103">windowsDefenderScanActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="29a89-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="29a89-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="29a89-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29a89-105">Letzte Analyseergebnisse von Windows Defender</span><span class="sxs-lookup"><span data-stu-id="29a89-105">Windows Defender last scan result</span></span>

<span data-ttu-id="29a89-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="29a89-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="29a89-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="29a89-107">Properties</span></span>
|<span data-ttu-id="29a89-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="29a89-108">Property</span></span>|<span data-ttu-id="29a89-109">Typ</span><span class="sxs-lookup"><span data-stu-id="29a89-109">Type</span></span>|<span data-ttu-id="29a89-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29a89-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29a89-111">actionName</span><span class="sxs-lookup"><span data-stu-id="29a89-111">actionName</span></span>|<span data-ttu-id="29a89-112">String</span><span class="sxs-lookup"><span data-stu-id="29a89-112">String</span></span>|<span data-ttu-id="29a89-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="29a89-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="29a89-114">actionState</span><span class="sxs-lookup"><span data-stu-id="29a89-114">actionState</span></span>|[<span data-ttu-id="29a89-115">actionState</span><span class="sxs-lookup"><span data-stu-id="29a89-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="29a89-116">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="29a89-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="29a89-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="29a89-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="29a89-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="29a89-118">startDateTime</span></span>|<span data-ttu-id="29a89-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29a89-119">DateTimeOffset</span></span>|<span data-ttu-id="29a89-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="29a89-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="29a89-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="29a89-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="29a89-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29a89-122">DateTimeOffset</span></span>|<span data-ttu-id="29a89-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="29a89-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="29a89-124">scanType</span><span class="sxs-lookup"><span data-stu-id="29a89-124">scanType</span></span>|<span data-ttu-id="29a89-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29a89-125">String</span></span>|<span data-ttu-id="29a89-126">Überprüfungstyp, entweder vollständige oder schnelle Überprüfung</span><span class="sxs-lookup"><span data-stu-id="29a89-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="29a89-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="29a89-127">Relationships</span></span>
<span data-ttu-id="29a89-128">Keine</span><span class="sxs-lookup"><span data-stu-id="29a89-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="29a89-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="29a89-129">JSON Representation</span></span>
<span data-ttu-id="29a89-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="29a89-130">Here is a JSON representation of the resource.</span></span>
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



