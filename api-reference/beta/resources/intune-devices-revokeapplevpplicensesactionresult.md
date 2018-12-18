---
title: Ressourcentyp revokeAppleVppLicensesActionResult
description: Apple Vpp Lizenzen Aktionsergebnis widerrufen
author: tfitzmac
ms.openlocfilehash: b45a2ddec46ddc5cac47937cb776d0f0da6c64a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361047"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="e43bf-103">Ressourcentyp revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="e43bf-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="e43bf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e43bf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e43bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e43bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e43bf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e43bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e43bf-107">Apple Vpp Lizenzen Aktionsergebnis widerrufen</span><span class="sxs-lookup"><span data-stu-id="e43bf-107">Revoke Apple Vpp licenses action result</span></span>

<span data-ttu-id="e43bf-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e43bf-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e43bf-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e43bf-109">Properties</span></span>
|<span data-ttu-id="e43bf-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e43bf-110">Property</span></span>|<span data-ttu-id="e43bf-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e43bf-111">Type</span></span>|<span data-ttu-id="e43bf-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e43bf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e43bf-113">actionName</span><span class="sxs-lookup"><span data-stu-id="e43bf-113">actionName</span></span>|<span data-ttu-id="e43bf-114">String</span><span class="sxs-lookup"><span data-stu-id="e43bf-114">String</span></span>|<span data-ttu-id="e43bf-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e43bf-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e43bf-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e43bf-116">actionState</span></span>|[<span data-ttu-id="e43bf-117">actionState</span><span class="sxs-lookup"><span data-stu-id="e43bf-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="e43bf-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="e43bf-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="e43bf-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="e43bf-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e43bf-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e43bf-120">startDateTime</span></span>|<span data-ttu-id="e43bf-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e43bf-121">DateTimeOffset</span></span>|<span data-ttu-id="e43bf-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e43bf-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e43bf-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e43bf-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="e43bf-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e43bf-124">DateTimeOffset</span></span>|<span data-ttu-id="e43bf-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e43bf-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e43bf-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="e43bf-126">totalLicensesCount</span></span>|<span data-ttu-id="e43bf-127">Int32</span><span class="sxs-lookup"><span data-stu-id="e43bf-127">Int32</span></span>|<span data-ttu-id="e43bf-128">Gesamtzahl der Apple Vpp Lizenzen verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="e43bf-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="e43bf-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="e43bf-129">failedLicensesCount</span></span>|<span data-ttu-id="e43bf-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e43bf-130">Int32</span></span>|<span data-ttu-id="e43bf-131">Gesamtzahl der Apple Vpp-Lizenzen, die nicht widerrufen</span><span class="sxs-lookup"><span data-stu-id="e43bf-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="e43bf-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e43bf-132">Relationships</span></span>
<span data-ttu-id="e43bf-133">Keine</span><span class="sxs-lookup"><span data-stu-id="e43bf-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e43bf-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e43bf-134">JSON Representation</span></span>
<span data-ttu-id="e43bf-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e43bf-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```





