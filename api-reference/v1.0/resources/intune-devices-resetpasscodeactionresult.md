---
title: resetPasscodeActionResult-Ressourcentyp
description: Kennung zurücksetzen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 81a30b36ac418d5553c7387fea22a172926a73ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824857"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="e0093-103">resetPasscodeActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e0093-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="e0093-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e0093-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0093-105">Kennung zurücksetzen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="e0093-105">Reset passcode action result</span></span>

<span data-ttu-id="e0093-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e0093-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0093-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e0093-107">Properties</span></span>
|<span data-ttu-id="e0093-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0093-108">Property</span></span>|<span data-ttu-id="e0093-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e0093-109">Type</span></span>|<span data-ttu-id="e0093-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0093-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0093-111">actionName</span><span class="sxs-lookup"><span data-stu-id="e0093-111">actionName</span></span>|<span data-ttu-id="e0093-112">String</span><span class="sxs-lookup"><span data-stu-id="e0093-112">String</span></span>|<span data-ttu-id="e0093-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e0093-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e0093-114">actionState</span><span class="sxs-lookup"><span data-stu-id="e0093-114">actionState</span></span>|[<span data-ttu-id="e0093-115">actionState</span><span class="sxs-lookup"><span data-stu-id="e0093-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="e0093-116">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="e0093-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="e0093-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="e0093-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e0093-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e0093-118">startDateTime</span></span>|<span data-ttu-id="e0093-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0093-119">DateTimeOffset</span></span>|<span data-ttu-id="e0093-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e0093-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e0093-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0093-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="e0093-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0093-122">DateTimeOffset</span></span>|<span data-ttu-id="e0093-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e0093-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e0093-124">Zugangscode</span><span class="sxs-lookup"><span data-stu-id="e0093-124">passcode</span></span>|<span data-ttu-id="e0093-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e0093-125">String</span></span>|<span data-ttu-id="e0093-126">Neu erstellter Zugangscode für das Gerät</span><span class="sxs-lookup"><span data-stu-id="e0093-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="e0093-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e0093-127">Relationships</span></span>
<span data-ttu-id="e0093-128">Keine</span><span class="sxs-lookup"><span data-stu-id="e0093-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e0093-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e0093-129">JSON Representation</span></span>
<span data-ttu-id="e0093-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e0093-130">Here is a JSON representation of the resource.</span></span>
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



