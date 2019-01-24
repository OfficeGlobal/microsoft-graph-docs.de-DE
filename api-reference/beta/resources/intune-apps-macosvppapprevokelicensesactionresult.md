---
title: Ressourcentyp macOsVppAppRevokeLicensesActionResult
description: Ergebnisse für Aktionen auf Mac OS Vpp Apps definiert, geerbte Eigenschaften für ActionResult enthält.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f90bd55476bbbb48ab3a4904886a67b217ab67b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429958"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="4d788-103">Ressourcentyp macOsVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="4d788-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="4d788-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4d788-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4d788-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d788-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d788-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d788-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d788-107">Ergebnisse für Aktionen auf Mac OS Vpp Apps definiert, geerbte Eigenschaften für ActionResult enthält.</span><span class="sxs-lookup"><span data-stu-id="4d788-107">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="4d788-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4d788-108">Properties</span></span>
|<span data-ttu-id="4d788-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d788-109">Property</span></span>|<span data-ttu-id="4d788-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4d788-110">Type</span></span>|<span data-ttu-id="4d788-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d788-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d788-112">userId</span><span class="sxs-lookup"><span data-stu-id="4d788-112">userId</span></span>|<span data-ttu-id="4d788-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d788-113">String</span></span>|<span data-ttu-id="4d788-114">Benutzer-ID der Aktion zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="4d788-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="4d788-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="4d788-115">managedDeviceId</span></span>|<span data-ttu-id="4d788-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d788-116">String</span></span>|<span data-ttu-id="4d788-117">Geräte-ID der Aktion zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="4d788-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="4d788-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="4d788-118">totalLicensesCount</span></span>|<span data-ttu-id="4d788-119">Int32</span><span class="sxs-lookup"><span data-stu-id="4d788-119">Int32</span></span>|<span data-ttu-id="4d788-120">Anzahl der Anzahl der Lizenzen, die für die Revoke versucht wurde.</span><span class="sxs-lookup"><span data-stu-id="4d788-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="4d788-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="4d788-121">failedLicensesCount</span></span>|<span data-ttu-id="4d788-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4d788-122">Int32</span></span>|<span data-ttu-id="4d788-123">Anzahl der Anzahl von Lizenzen für welche Revoke ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="4d788-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="4d788-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="4d788-124">actionFailureReason</span></span>|[<span data-ttu-id="4d788-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="4d788-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="4d788-126">Der Grund für das Revoke Lizenzen-Aktion fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="4d788-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="4d788-127">Mögliche Werte sind: `none`, `appleFailure`, `internalError`, `expiredVppToken` und `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="4d788-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="4d788-128">actionName</span><span class="sxs-lookup"><span data-stu-id="4d788-128">actionName</span></span>|<span data-ttu-id="4d788-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d788-129">String</span></span>|<span data-ttu-id="4d788-130">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="4d788-130">Action name</span></span>|
|<span data-ttu-id="4d788-131">actionState</span><span class="sxs-lookup"><span data-stu-id="4d788-131">actionState</span></span>|[<span data-ttu-id="4d788-132">actionState</span><span class="sxs-lookup"><span data-stu-id="4d788-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4d788-133">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="4d788-133">State of the action.</span></span> <span data-ttu-id="4d788-134">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4d788-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4d788-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4d788-135">startDateTime</span></span>|<span data-ttu-id="4d788-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d788-136">DateTimeOffset</span></span>|<span data-ttu-id="4d788-137">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="4d788-137">Time the action was initiated</span></span>|
|<span data-ttu-id="4d788-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d788-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="4d788-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d788-139">DateTimeOffset</span></span>|<span data-ttu-id="4d788-140">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="4d788-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d788-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4d788-141">Relationships</span></span>
<span data-ttu-id="4d788-142">Keine</span><span class="sxs-lookup"><span data-stu-id="4d788-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d788-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4d788-143">JSON Representation</span></span>
<span data-ttu-id="4d788-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d788-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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



