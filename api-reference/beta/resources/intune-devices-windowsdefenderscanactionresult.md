---
title: windowsDefenderScanActionResult-Ressourcentyp
description: Letzte Analyseergebnisse von Windows Defender
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 913c821b60feb4901d812f2055c72e028537dd12
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405499"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="07561-103">windowsDefenderScanActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="07561-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="07561-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="07561-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07561-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07561-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07561-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07561-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07561-107">Letzte Analyseergebnisse von Windows Defender</span><span class="sxs-lookup"><span data-stu-id="07561-107">Windows Defender last scan result</span></span>


<span data-ttu-id="07561-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="07561-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="07561-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07561-109">Properties</span></span>
|<span data-ttu-id="07561-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07561-110">Property</span></span>|<span data-ttu-id="07561-111">Typ</span><span class="sxs-lookup"><span data-stu-id="07561-111">Type</span></span>|<span data-ttu-id="07561-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07561-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07561-113">actionName</span><span class="sxs-lookup"><span data-stu-id="07561-113">actionName</span></span>|<span data-ttu-id="07561-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07561-114">String</span></span>|<span data-ttu-id="07561-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="07561-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="07561-116">actionState</span><span class="sxs-lookup"><span data-stu-id="07561-116">actionState</span></span>|[<span data-ttu-id="07561-117">actionState</span><span class="sxs-lookup"><span data-stu-id="07561-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="07561-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="07561-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="07561-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="07561-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="07561-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="07561-120">startDateTime</span></span>|<span data-ttu-id="07561-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07561-121">DateTimeOffset</span></span>|<span data-ttu-id="07561-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="07561-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="07561-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="07561-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="07561-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07561-124">DateTimeOffset</span></span>|<span data-ttu-id="07561-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="07561-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="07561-126">scanType</span><span class="sxs-lookup"><span data-stu-id="07561-126">scanType</span></span>|<span data-ttu-id="07561-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07561-127">String</span></span>|<span data-ttu-id="07561-128">Überprüfungstyp, entweder vollständige oder schnelle Überprüfung</span><span class="sxs-lookup"><span data-stu-id="07561-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="07561-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="07561-129">Relationships</span></span>
<span data-ttu-id="07561-130">Keine</span><span class="sxs-lookup"><span data-stu-id="07561-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07561-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07561-131">JSON Representation</span></span>
<span data-ttu-id="07561-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07561-132">Here is a JSON representation of the resource.</span></span>
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




