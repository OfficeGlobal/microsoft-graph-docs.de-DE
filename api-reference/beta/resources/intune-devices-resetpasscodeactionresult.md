---
title: resetPasscodeActionResult-Ressourcentyp
description: Kennung zurücksetzen – Aktionsergebnis
author: tfitzmac
ms.openlocfilehash: 24d7a6f259f456c742c4317763dd9cefe8d185a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301111"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="a58dd-103">resetPasscodeActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a58dd-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="a58dd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a58dd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a58dd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a58dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a58dd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a58dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a58dd-107">Kennung zurücksetzen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="a58dd-107">Reset passcode action result</span></span>

<span data-ttu-id="a58dd-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a58dd-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a58dd-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a58dd-109">Properties</span></span>
|<span data-ttu-id="a58dd-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a58dd-110">Property</span></span>|<span data-ttu-id="a58dd-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a58dd-111">Type</span></span>|<span data-ttu-id="a58dd-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a58dd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a58dd-113">actionName</span><span class="sxs-lookup"><span data-stu-id="a58dd-113">actionName</span></span>|<span data-ttu-id="a58dd-114">String</span><span class="sxs-lookup"><span data-stu-id="a58dd-114">String</span></span>|<span data-ttu-id="a58dd-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a58dd-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a58dd-116">actionState</span><span class="sxs-lookup"><span data-stu-id="a58dd-116">actionState</span></span>|[<span data-ttu-id="a58dd-117">actionState</span><span class="sxs-lookup"><span data-stu-id="a58dd-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a58dd-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a58dd-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="a58dd-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a58dd-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a58dd-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a58dd-120">startDateTime</span></span>|<span data-ttu-id="a58dd-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a58dd-121">DateTimeOffset</span></span>|<span data-ttu-id="a58dd-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a58dd-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a58dd-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a58dd-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="a58dd-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a58dd-124">DateTimeOffset</span></span>|<span data-ttu-id="a58dd-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a58dd-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a58dd-126">Zugangscode</span><span class="sxs-lookup"><span data-stu-id="a58dd-126">passcode</span></span>|<span data-ttu-id="a58dd-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a58dd-127">String</span></span>|<span data-ttu-id="a58dd-128">Neu erstellter Zugangscode für das Gerät</span><span class="sxs-lookup"><span data-stu-id="a58dd-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="a58dd-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a58dd-129">Relationships</span></span>
<span data-ttu-id="a58dd-130">Keine</span><span class="sxs-lookup"><span data-stu-id="a58dd-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a58dd-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a58dd-131">JSON Representation</span></span>
<span data-ttu-id="a58dd-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a58dd-132">Here is a JSON representation of the resource.</span></span>
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





