---
title: revokeAppleVppLicensesActionResult-Ressourcentyp
description: Widerrufen von Apple VPP-Lizenzen-aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6590ae51f88c5bb00318e5e5be3769afdf629edf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146487"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="b80b5-103">revokeAppleVppLicensesActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b80b5-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="b80b5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b80b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b80b5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b80b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b80b5-106">Widerrufen von Apple VPP-Lizenzen-aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="b80b5-106">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="b80b5-107">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b80b5-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b80b5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b80b5-108">Properties</span></span>
|<span data-ttu-id="b80b5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b80b5-109">Property</span></span>|<span data-ttu-id="b80b5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b80b5-110">Type</span></span>|<span data-ttu-id="b80b5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b80b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b80b5-112">actionName</span><span class="sxs-lookup"><span data-stu-id="b80b5-112">actionName</span></span>|<span data-ttu-id="b80b5-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b80b5-113">String</span></span>|<span data-ttu-id="b80b5-114">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b80b5-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b80b5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b80b5-115">actionState</span></span>|[<span data-ttu-id="b80b5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b80b5-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b80b5-117">Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="b80b5-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b80b5-118">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b80b5-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b80b5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b80b5-119">startDateTime</span></span>|<span data-ttu-id="b80b5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b80b5-120">DateTimeOffset</span></span>|<span data-ttu-id="b80b5-121">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b80b5-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b80b5-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b80b5-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="b80b5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b80b5-123">DateTimeOffset</span></span>|<span data-ttu-id="b80b5-124">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b80b5-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b80b5-125">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="b80b5-125">totalLicensesCount</span></span>|<span data-ttu-id="b80b5-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b80b5-126">Int32</span></span>|<span data-ttu-id="b80b5-127">Gesamtzahl der zugeordneten Apple VPP-Lizenzen</span><span class="sxs-lookup"><span data-stu-id="b80b5-127">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="b80b5-128">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="b80b5-128">failedLicensesCount</span></span>|<span data-ttu-id="b80b5-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b80b5-129">Int32</span></span>|<span data-ttu-id="b80b5-130">Gesamtzahl der Apple VPP-Lizenzen, die nicht widerrufen werden konnten</span><span class="sxs-lookup"><span data-stu-id="b80b5-130">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="b80b5-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b80b5-131">Relationships</span></span>
<span data-ttu-id="b80b5-132">Keine</span><span class="sxs-lookup"><span data-stu-id="b80b5-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b80b5-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b80b5-133">JSON Representation</span></span>
<span data-ttu-id="b80b5-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b80b5-134">Here is a JSON representation of the resource.</span></span>
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




