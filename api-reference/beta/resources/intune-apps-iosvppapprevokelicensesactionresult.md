---
title: iosVppAppRevokeLicensesActionResult-Ressourcentyp
description: Definiert Ergebnisse für Aktionen bei iOS-VPP-apps, enthält geerbte Eigenschaften für ActionResult.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 542382411fcc1070dc0c397efbf43431081d73f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153452"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="6a8bb-103">iosVppAppRevokeLicensesActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6a8bb-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="6a8bb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a8bb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a8bb-106">Definiert Ergebnisse für Aktionen bei iOS-VPP-apps, enthält geerbte Eigenschaften für ActionResult.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-106">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="6a8bb-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6a8bb-107">Properties</span></span>
|<span data-ttu-id="6a8bb-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a8bb-108">Property</span></span>|<span data-ttu-id="6a8bb-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6a8bb-109">Type</span></span>|<span data-ttu-id="6a8bb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a8bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a8bb-111">userId</span><span class="sxs-lookup"><span data-stu-id="6a8bb-111">userId</span></span>|<span data-ttu-id="6a8bb-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a8bb-112">String</span></span>|<span data-ttu-id="6a8bb-113">Der Aktion zugeordnete UserId.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="6a8bb-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="6a8bb-114">managedDeviceId</span></span>|<span data-ttu-id="6a8bb-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a8bb-115">String</span></span>|<span data-ttu-id="6a8bb-116">Mit der Aktion verknüpfte Geräte-Nr.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="6a8bb-117">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="6a8bb-117">totalLicensesCount</span></span>|<span data-ttu-id="6a8bb-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6a8bb-118">Int32</span></span>|<span data-ttu-id="6a8bb-119">Die Anzahl der Lizenzen, für die widerrufen versucht wurde.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="6a8bb-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="6a8bb-120">failedLicensesCount</span></span>|<span data-ttu-id="6a8bb-121">Int32</span><span class="sxs-lookup"><span data-stu-id="6a8bb-121">Int32</span></span>|<span data-ttu-id="6a8bb-122">Die Anzahl der Lizenzen, für die REVOKE fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="6a8bb-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="6a8bb-123">actionFailureReason</span></span>|[<span data-ttu-id="6a8bb-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="6a8bb-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="6a8bb-125">Der Grund für den Fehlschlagen der Lizenz Widerruf.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="6a8bb-126">Mögliche Werte: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="6a8bb-127">actionName</span><span class="sxs-lookup"><span data-stu-id="6a8bb-127">actionName</span></span>|<span data-ttu-id="6a8bb-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a8bb-128">String</span></span>|<span data-ttu-id="6a8bb-129">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="6a8bb-129">Action name</span></span>|
|<span data-ttu-id="6a8bb-130">actionState</span><span class="sxs-lookup"><span data-stu-id="6a8bb-130">actionState</span></span>|[<span data-ttu-id="6a8bb-131">actionState</span><span class="sxs-lookup"><span data-stu-id="6a8bb-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6a8bb-132">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-132">State of the action.</span></span> <span data-ttu-id="6a8bb-133">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6a8bb-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6a8bb-134">startDateTime</span></span>|<span data-ttu-id="6a8bb-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a8bb-135">DateTimeOffset</span></span>|<span data-ttu-id="6a8bb-136">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="6a8bb-136">Time the action was initiated</span></span>|
|<span data-ttu-id="6a8bb-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a8bb-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="6a8bb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a8bb-138">DateTimeOffset</span></span>|<span data-ttu-id="6a8bb-139">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="6a8bb-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a8bb-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6a8bb-140">Relationships</span></span>
<span data-ttu-id="6a8bb-141">Keine</span><span class="sxs-lookup"><span data-stu-id="6a8bb-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a8bb-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6a8bb-142">JSON Representation</span></span>
<span data-ttu-id="6a8bb-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6a8bb-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppRevokeLicensesActionResult",
  "userId": "String",
  "managedDeviceId": "String",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




