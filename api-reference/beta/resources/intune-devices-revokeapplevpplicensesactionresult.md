---
title: Ressourcentyp revokeAppleVppLicensesActionResult
description: Apple Vpp Lizenzen Aktionsergebnis widerrufen
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cd77bee330e919ab51927af0773d913099cea6e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419226"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="e3b96-103">Ressourcentyp revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="e3b96-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="e3b96-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e3b96-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e3b96-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3b96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3b96-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3b96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3b96-107">Apple Vpp Lizenzen Aktionsergebnis widerrufen</span><span class="sxs-lookup"><span data-stu-id="e3b96-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="e3b96-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e3b96-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e3b96-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3b96-109">Properties</span></span>
|<span data-ttu-id="e3b96-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3b96-110">Property</span></span>|<span data-ttu-id="e3b96-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e3b96-111">Type</span></span>|<span data-ttu-id="e3b96-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3b96-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3b96-113">actionName</span><span class="sxs-lookup"><span data-stu-id="e3b96-113">actionName</span></span>|<span data-ttu-id="e3b96-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3b96-114">String</span></span>|<span data-ttu-id="e3b96-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e3b96-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e3b96-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e3b96-116">actionState</span></span>|[<span data-ttu-id="e3b96-117">actionState</span><span class="sxs-lookup"><span data-stu-id="e3b96-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="e3b96-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="e3b96-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="e3b96-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="e3b96-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e3b96-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e3b96-120">startDateTime</span></span>|<span data-ttu-id="e3b96-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3b96-121">DateTimeOffset</span></span>|<span data-ttu-id="e3b96-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e3b96-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e3b96-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3b96-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="e3b96-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3b96-124">DateTimeOffset</span></span>|<span data-ttu-id="e3b96-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e3b96-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e3b96-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="e3b96-126">totalLicensesCount</span></span>|<span data-ttu-id="e3b96-127">Int32</span><span class="sxs-lookup"><span data-stu-id="e3b96-127">Int32</span></span>|<span data-ttu-id="e3b96-128">Gesamtzahl der Apple Vpp Lizenzen verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="e3b96-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="e3b96-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="e3b96-129">failedLicensesCount</span></span>|<span data-ttu-id="e3b96-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e3b96-130">Int32</span></span>|<span data-ttu-id="e3b96-131">Gesamtzahl der Apple Vpp-Lizenzen, die nicht widerrufen</span><span class="sxs-lookup"><span data-stu-id="e3b96-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3b96-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e3b96-132">Relationships</span></span>
<span data-ttu-id="e3b96-133">Keine</span><span class="sxs-lookup"><span data-stu-id="e3b96-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3b96-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3b96-134">JSON Representation</span></span>
<span data-ttu-id="e3b96-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3b96-135">Here is a JSON representation of the resource.</span></span>
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




