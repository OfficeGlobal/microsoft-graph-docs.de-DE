---
title: resetPasscodeActionResult-Ressourcentyp
description: Kennung zurücksetzen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e23c3e7d39566df98ab57258a54ab6f637439d1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257001"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="9934d-103">resetPasscodeActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9934d-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="9934d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9934d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9934d-105">Kennung zurücksetzen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="9934d-105">Reset passcode action result</span></span>


<span data-ttu-id="9934d-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9934d-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9934d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9934d-107">Properties</span></span>
|<span data-ttu-id="9934d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9934d-108">Property</span></span>|<span data-ttu-id="9934d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9934d-109">Type</span></span>|<span data-ttu-id="9934d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9934d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9934d-111">actionName</span><span class="sxs-lookup"><span data-stu-id="9934d-111">actionName</span></span>|<span data-ttu-id="9934d-112">String</span><span class="sxs-lookup"><span data-stu-id="9934d-112">String</span></span>|<span data-ttu-id="9934d-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9934d-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9934d-114">actionState</span><span class="sxs-lookup"><span data-stu-id="9934d-114">actionState</span></span>|[<span data-ttu-id="9934d-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9934d-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="9934d-116">Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="9934d-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9934d-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9934d-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9934d-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9934d-118">startDateTime</span></span>|<span data-ttu-id="9934d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9934d-119">DateTimeOffset</span></span>|<span data-ttu-id="9934d-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9934d-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9934d-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9934d-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="9934d-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9934d-122">DateTimeOffset</span></span>|<span data-ttu-id="9934d-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9934d-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9934d-124">Zugangscode</span><span class="sxs-lookup"><span data-stu-id="9934d-124">passcode</span></span>|<span data-ttu-id="9934d-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9934d-125">String</span></span>|<span data-ttu-id="9934d-126">Neu erstellter Zugangscode für das Gerät</span><span class="sxs-lookup"><span data-stu-id="9934d-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="9934d-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9934d-127">Relationships</span></span>
<span data-ttu-id="9934d-128">Keine</span><span class="sxs-lookup"><span data-stu-id="9934d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9934d-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9934d-129">JSON Representation</span></span>
<span data-ttu-id="9934d-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9934d-130">Here is a JSON representation of the resource.</span></span>
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



