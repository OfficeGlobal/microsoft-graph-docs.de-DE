---
title: remoteLockActionResult-Ressourcentyp
description: Ergebnis einer Sperraktion mit einem Pin zum Entsperren
ms.openlocfilehash: 39791c2e20d39a8fced01a16c6cf0cea0c0db4cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058214"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="936c1-103">remoteLockActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="936c1-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="936c1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="936c1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="936c1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="936c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="936c1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="936c1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="936c1-107">Ergebnis einer Sperraktion mit einem Pin zum Entsperren</span><span class="sxs-lookup"><span data-stu-id="936c1-107">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="936c1-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="936c1-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="936c1-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="936c1-109">Properties</span></span>
|<span data-ttu-id="936c1-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="936c1-110">Property</span></span>|<span data-ttu-id="936c1-111">Typ</span><span class="sxs-lookup"><span data-stu-id="936c1-111">Type</span></span>|<span data-ttu-id="936c1-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="936c1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="936c1-113">actionName</span><span class="sxs-lookup"><span data-stu-id="936c1-113">actionName</span></span>|<span data-ttu-id="936c1-114">String</span><span class="sxs-lookup"><span data-stu-id="936c1-114">String</span></span>|<span data-ttu-id="936c1-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="936c1-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="936c1-116">actionState</span><span class="sxs-lookup"><span data-stu-id="936c1-116">actionState</span></span>|[<span data-ttu-id="936c1-117">actionState</span><span class="sxs-lookup"><span data-stu-id="936c1-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="936c1-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="936c1-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="936c1-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="936c1-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="936c1-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="936c1-120">startDateTime</span></span>|<span data-ttu-id="936c1-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="936c1-121">DateTimeOffset</span></span>|<span data-ttu-id="936c1-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="936c1-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="936c1-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="936c1-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="936c1-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="936c1-124">DateTimeOffset</span></span>|<span data-ttu-id="936c1-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="936c1-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="936c1-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="936c1-126">unlockPin</span></span>|<span data-ttu-id="936c1-127">String</span><span class="sxs-lookup"><span data-stu-id="936c1-127">String</span></span>|<span data-ttu-id="936c1-128">Pin zum Entsperren des Clients</span><span class="sxs-lookup"><span data-stu-id="936c1-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="936c1-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="936c1-129">Relationships</span></span>
<span data-ttu-id="936c1-130">Keine</span><span class="sxs-lookup"><span data-stu-id="936c1-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="936c1-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="936c1-131">JSON Representation</span></span>
<span data-ttu-id="936c1-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="936c1-132">Here is a JSON representation of the resource.</span></span>
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





