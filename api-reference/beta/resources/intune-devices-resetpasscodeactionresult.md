---
title: resetPasscodeActionResult-Ressourcentyp
description: Kennung zurücksetzen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f4090309cb059c1f8cddca77cb787ff69f54c7f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172037"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="e3882-103">resetPasscodeActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e3882-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="e3882-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3882-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3882-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e3882-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3882-106">Kennung zurücksetzen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="e3882-106">Reset passcode action result</span></span>


<span data-ttu-id="e3882-107">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e3882-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e3882-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3882-108">Properties</span></span>
|<span data-ttu-id="e3882-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3882-109">Property</span></span>|<span data-ttu-id="e3882-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e3882-110">Type</span></span>|<span data-ttu-id="e3882-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3882-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3882-112">actionName</span><span class="sxs-lookup"><span data-stu-id="e3882-112">actionName</span></span>|<span data-ttu-id="e3882-113">String</span><span class="sxs-lookup"><span data-stu-id="e3882-113">String</span></span>|<span data-ttu-id="e3882-114">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e3882-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e3882-115">actionState</span><span class="sxs-lookup"><span data-stu-id="e3882-115">actionState</span></span>|[<span data-ttu-id="e3882-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e3882-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="e3882-117">Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="e3882-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="e3882-118">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="e3882-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e3882-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e3882-119">startDateTime</span></span>|<span data-ttu-id="e3882-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3882-120">DateTimeOffset</span></span>|<span data-ttu-id="e3882-121">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e3882-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e3882-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3882-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="e3882-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3882-123">DateTimeOffset</span></span>|<span data-ttu-id="e3882-124">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e3882-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e3882-125">Zugangscode</span><span class="sxs-lookup"><span data-stu-id="e3882-125">passcode</span></span>|<span data-ttu-id="e3882-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3882-126">String</span></span>|<span data-ttu-id="e3882-127">Neu erstellter Zugangscode für das Gerät</span><span class="sxs-lookup"><span data-stu-id="e3882-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="e3882-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e3882-128">Relationships</span></span>
<span data-ttu-id="e3882-129">Keine</span><span class="sxs-lookup"><span data-stu-id="e3882-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3882-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3882-130">JSON Representation</span></span>
<span data-ttu-id="e3882-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3882-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```




