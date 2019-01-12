---
title: resetPasscodeActionResult-Ressourcentyp
description: Kennung zurücksetzen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e526370ca86792ed30a5f5e24a4be244d73441b6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920842"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="09724-103">resetPasscodeActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="09724-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="09724-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="09724-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09724-105">Kennung zurücksetzen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="09724-105">Reset passcode action result</span></span>

<span data-ttu-id="09724-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="09724-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09724-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="09724-107">Properties</span></span>
|<span data-ttu-id="09724-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="09724-108">Property</span></span>|<span data-ttu-id="09724-109">Typ</span><span class="sxs-lookup"><span data-stu-id="09724-109">Type</span></span>|<span data-ttu-id="09724-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09724-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09724-111">actionName</span><span class="sxs-lookup"><span data-stu-id="09724-111">actionName</span></span>|<span data-ttu-id="09724-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09724-112">String</span></span>|<span data-ttu-id="09724-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="09724-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="09724-114">actionState</span><span class="sxs-lookup"><span data-stu-id="09724-114">actionState</span></span>|[<span data-ttu-id="09724-115">actionState</span><span class="sxs-lookup"><span data-stu-id="09724-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="09724-116">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="09724-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="09724-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="09724-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="09724-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="09724-118">startDateTime</span></span>|<span data-ttu-id="09724-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09724-119">DateTimeOffset</span></span>|<span data-ttu-id="09724-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="09724-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="09724-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="09724-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="09724-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09724-122">DateTimeOffset</span></span>|<span data-ttu-id="09724-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="09724-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="09724-124">Zugangscode</span><span class="sxs-lookup"><span data-stu-id="09724-124">passcode</span></span>|<span data-ttu-id="09724-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09724-125">String</span></span>|<span data-ttu-id="09724-126">Neu erstellter Zugangscode für das Gerät</span><span class="sxs-lookup"><span data-stu-id="09724-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="09724-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="09724-127">Relationships</span></span>
<span data-ttu-id="09724-128">Keine</span><span class="sxs-lookup"><span data-stu-id="09724-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09724-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="09724-129">JSON Representation</span></span>
<span data-ttu-id="09724-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="09724-130">Here is a JSON representation of the resource.</span></span>
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



