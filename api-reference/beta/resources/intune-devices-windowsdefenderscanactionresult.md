---
title: windowsDefenderScanActionResult-Ressourcentyp
description: Letzte Analyseergebnisse von Windows Defender
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5ac1f35473b69afab3b4609f2798945d40f169bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846536"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="413ef-103">windowsDefenderScanActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="413ef-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="413ef-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="413ef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="413ef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="413ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="413ef-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="413ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="413ef-107">Letzte Analyseergebnisse von Windows Defender</span><span class="sxs-lookup"><span data-stu-id="413ef-107">Windows Defender last scan result</span></span>

<span data-ttu-id="413ef-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="413ef-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="413ef-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="413ef-109">Properties</span></span>
|<span data-ttu-id="413ef-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="413ef-110">Property</span></span>|<span data-ttu-id="413ef-111">Typ</span><span class="sxs-lookup"><span data-stu-id="413ef-111">Type</span></span>|<span data-ttu-id="413ef-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="413ef-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="413ef-113">actionName</span><span class="sxs-lookup"><span data-stu-id="413ef-113">actionName</span></span>|<span data-ttu-id="413ef-114">String</span><span class="sxs-lookup"><span data-stu-id="413ef-114">String</span></span>|<span data-ttu-id="413ef-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="413ef-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="413ef-116">actionState</span><span class="sxs-lookup"><span data-stu-id="413ef-116">actionState</span></span>|[<span data-ttu-id="413ef-117">actionState</span><span class="sxs-lookup"><span data-stu-id="413ef-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="413ef-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="413ef-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="413ef-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="413ef-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="413ef-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="413ef-120">startDateTime</span></span>|<span data-ttu-id="413ef-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="413ef-121">DateTimeOffset</span></span>|<span data-ttu-id="413ef-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="413ef-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="413ef-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="413ef-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="413ef-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="413ef-124">DateTimeOffset</span></span>|<span data-ttu-id="413ef-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="413ef-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="413ef-126">scanType</span><span class="sxs-lookup"><span data-stu-id="413ef-126">scanType</span></span>|<span data-ttu-id="413ef-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="413ef-127">String</span></span>|<span data-ttu-id="413ef-128">Überprüfungstyp, entweder vollständige oder schnelle Überprüfung</span><span class="sxs-lookup"><span data-stu-id="413ef-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="413ef-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="413ef-129">Relationships</span></span>
<span data-ttu-id="413ef-130">Keine</span><span class="sxs-lookup"><span data-stu-id="413ef-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="413ef-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="413ef-131">JSON Representation</span></span>
<span data-ttu-id="413ef-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="413ef-132">Here is a JSON representation of the resource.</span></span>
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





