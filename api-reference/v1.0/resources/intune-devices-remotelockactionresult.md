---
title: remoteLockActionResult-Ressourcentyp
description: Ergebnis einer Sperraktion mit einem Pin zum Entsperren
author: tfitzmac
ms.openlocfilehash: 44d56b2ee20629d1cefbf965c72e5f6cc17fb0a2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353690"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="8e7f9-103">remoteLockActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8e7f9-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="8e7f9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e7f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e7f9-105">Ergebnis einer Sperraktion mit einem Pin zum Entsperren</span><span class="sxs-lookup"><span data-stu-id="8e7f9-105">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="8e7f9-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8e7f9-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e7f9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8e7f9-107">Properties</span></span>
|<span data-ttu-id="8e7f9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e7f9-108">Property</span></span>|<span data-ttu-id="8e7f9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8e7f9-109">Type</span></span>|<span data-ttu-id="8e7f9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e7f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e7f9-111">actionName</span><span class="sxs-lookup"><span data-stu-id="8e7f9-111">actionName</span></span>|<span data-ttu-id="8e7f9-112">String</span><span class="sxs-lookup"><span data-stu-id="8e7f9-112">String</span></span>|<span data-ttu-id="8e7f9-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8e7f9-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8e7f9-114">actionState</span><span class="sxs-lookup"><span data-stu-id="8e7f9-114">actionState</span></span>|[<span data-ttu-id="8e7f9-115">actionState</span><span class="sxs-lookup"><span data-stu-id="8e7f9-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="8e7f9-116">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="8e7f9-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="8e7f9-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8e7f9-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8e7f9-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8e7f9-118">startDateTime</span></span>|<span data-ttu-id="8e7f9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e7f9-119">DateTimeOffset</span></span>|<span data-ttu-id="8e7f9-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8e7f9-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8e7f9-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e7f9-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="8e7f9-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e7f9-122">DateTimeOffset</span></span>|<span data-ttu-id="8e7f9-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8e7f9-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8e7f9-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="8e7f9-124">unlockPin</span></span>|<span data-ttu-id="8e7f9-125">String</span><span class="sxs-lookup"><span data-stu-id="8e7f9-125">String</span></span>|<span data-ttu-id="8e7f9-126">Pin zum Entsperren des Clients</span><span class="sxs-lookup"><span data-stu-id="8e7f9-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e7f9-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8e7f9-127">Relationships</span></span>
<span data-ttu-id="8e7f9-128">Keine</span><span class="sxs-lookup"><span data-stu-id="8e7f9-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e7f9-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8e7f9-129">JSON Representation</span></span>
<span data-ttu-id="8e7f9-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8e7f9-130">Here is a JSON representation of the resource.</span></span>
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



