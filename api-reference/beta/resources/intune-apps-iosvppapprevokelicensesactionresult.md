---
title: Ressourcentyp iosVppAppRevokeLicensesActionResult
description: Ergebnisse für Aktionen auf iOS Apps Vpp definiert, geerbte Eigenschaften für ActionResult enthält.
ms.openlocfilehash: 1c6c1486d63ba5ce7c866dc2697d1a3eb2ee8e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064893"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="9d1c6-103">Ressourcentyp iosVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="9d1c6-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="9d1c6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d1c6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d1c6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d1c6-107">Ergebnisse für Aktionen auf iOS Apps Vpp definiert, geerbte Eigenschaften für ActionResult enthält.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>
## <a name="properties"></a><span data-ttu-id="9d1c6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9d1c6-108">Properties</span></span>
|<span data-ttu-id="9d1c6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9d1c6-109">Property</span></span>|<span data-ttu-id="9d1c6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9d1c6-110">Type</span></span>|<span data-ttu-id="9d1c6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d1c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d1c6-112">userId</span><span class="sxs-lookup"><span data-stu-id="9d1c6-112">userId</span></span>|<span data-ttu-id="9d1c6-113">String</span><span class="sxs-lookup"><span data-stu-id="9d1c6-113">String</span></span>|<span data-ttu-id="9d1c6-114">Benutzer-ID der Aktion zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="9d1c6-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="9d1c6-115">managedDeviceId</span></span>|<span data-ttu-id="9d1c6-116">String</span><span class="sxs-lookup"><span data-stu-id="9d1c6-116">String</span></span>|<span data-ttu-id="9d1c6-117">Geräte-ID der Aktion zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="9d1c6-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="9d1c6-118">totalLicensesCount</span></span>|<span data-ttu-id="9d1c6-119">Int32</span><span class="sxs-lookup"><span data-stu-id="9d1c6-119">Int32</span></span>|<span data-ttu-id="9d1c6-120">Anzahl der Anzahl der Lizenzen, die für die Revoke versucht wurde.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="9d1c6-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="9d1c6-121">failedLicensesCount</span></span>|<span data-ttu-id="9d1c6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9d1c6-122">Int32</span></span>|<span data-ttu-id="9d1c6-123">Anzahl der Anzahl von Lizenzen für welche Revoke ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="9d1c6-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="9d1c6-124">actionFailureReason</span></span>|[<span data-ttu-id="9d1c6-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="9d1c6-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="9d1c6-126">Der Grund für das Revoke Lizenzen-Aktion fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="9d1c6-127">Mögliche Werte sind: `none`, `appleFailure`, `internalError`, `expiredVppToken` und `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="9d1c6-128">actionName</span><span class="sxs-lookup"><span data-stu-id="9d1c6-128">actionName</span></span>|<span data-ttu-id="9d1c6-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9d1c6-129">String</span></span>|<span data-ttu-id="9d1c6-130">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="9d1c6-130">Action name</span></span>|
|<span data-ttu-id="9d1c6-131">actionState</span><span class="sxs-lookup"><span data-stu-id="9d1c6-131">actionState</span></span>|[<span data-ttu-id="9d1c6-132">actionState</span><span class="sxs-lookup"><span data-stu-id="9d1c6-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9d1c6-133">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-133">State of the action.</span></span> <span data-ttu-id="9d1c6-134">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9d1c6-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9d1c6-135">startDateTime</span></span>|<span data-ttu-id="9d1c6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d1c6-136">DateTimeOffset</span></span>|<span data-ttu-id="9d1c6-137">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="9d1c6-137">Time the action was initiated</span></span>|
|<span data-ttu-id="9d1c6-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d1c6-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="9d1c6-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d1c6-139">DateTimeOffset</span></span>|<span data-ttu-id="9d1c6-140">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="9d1c6-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d1c6-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9d1c6-141">Relationships</span></span>
<span data-ttu-id="9d1c6-142">Keine</span><span class="sxs-lookup"><span data-stu-id="9d1c6-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9d1c6-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9d1c6-143">JSON Representation</span></span>
<span data-ttu-id="9d1c6-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9d1c6-144">Here is a JSON representation of the resource.</span></span>
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





