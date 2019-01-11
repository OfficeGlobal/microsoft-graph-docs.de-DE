---
title: Ressourcentyp revokeAppleVppLicensesActionResult
description: Apple Vpp Lizenzen Aktionsergebnis widerrufen
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b7e578ee695e171a1a91167b61e47af717dd82c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879100"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="881f9-103">Ressourcentyp revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="881f9-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="881f9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="881f9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="881f9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="881f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="881f9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="881f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="881f9-107">Apple Vpp Lizenzen Aktionsergebnis widerrufen</span><span class="sxs-lookup"><span data-stu-id="881f9-107">Revoke Apple Vpp licenses action result</span></span>

<span data-ttu-id="881f9-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="881f9-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="881f9-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="881f9-109">Properties</span></span>
|<span data-ttu-id="881f9-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="881f9-110">Property</span></span>|<span data-ttu-id="881f9-111">Typ</span><span class="sxs-lookup"><span data-stu-id="881f9-111">Type</span></span>|<span data-ttu-id="881f9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="881f9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="881f9-113">actionName</span><span class="sxs-lookup"><span data-stu-id="881f9-113">actionName</span></span>|<span data-ttu-id="881f9-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="881f9-114">String</span></span>|<span data-ttu-id="881f9-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="881f9-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="881f9-116">actionState</span><span class="sxs-lookup"><span data-stu-id="881f9-116">actionState</span></span>|[<span data-ttu-id="881f9-117">actionState</span><span class="sxs-lookup"><span data-stu-id="881f9-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="881f9-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="881f9-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="881f9-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="881f9-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="881f9-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="881f9-120">startDateTime</span></span>|<span data-ttu-id="881f9-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="881f9-121">DateTimeOffset</span></span>|<span data-ttu-id="881f9-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="881f9-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="881f9-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="881f9-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="881f9-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="881f9-124">DateTimeOffset</span></span>|<span data-ttu-id="881f9-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="881f9-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="881f9-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="881f9-126">totalLicensesCount</span></span>|<span data-ttu-id="881f9-127">Int32</span><span class="sxs-lookup"><span data-stu-id="881f9-127">Int32</span></span>|<span data-ttu-id="881f9-128">Gesamtzahl der Apple Vpp Lizenzen verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="881f9-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="881f9-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="881f9-129">failedLicensesCount</span></span>|<span data-ttu-id="881f9-130">Int32</span><span class="sxs-lookup"><span data-stu-id="881f9-130">Int32</span></span>|<span data-ttu-id="881f9-131">Gesamtzahl der Apple Vpp-Lizenzen, die nicht widerrufen</span><span class="sxs-lookup"><span data-stu-id="881f9-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="881f9-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="881f9-132">Relationships</span></span>
<span data-ttu-id="881f9-133">Keine</span><span class="sxs-lookup"><span data-stu-id="881f9-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="881f9-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="881f9-134">JSON Representation</span></span>
<span data-ttu-id="881f9-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="881f9-135">Here is a JSON representation of the resource.</span></span>
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





