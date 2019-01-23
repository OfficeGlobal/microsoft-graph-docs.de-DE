---
title: Ressourcentyp vppTokenRevokeLicensesActionResult
description: Der Status der Aktion Revoke-Lizenzen für das Token Apple Volume Purchase Program ausgeführt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75c75c6b8bcdc06ede0f71b19956155becc4d478
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418225"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="6f378-103">Ressourcentyp vppTokenRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="6f378-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="6f378-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6f378-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f378-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f378-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f378-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f378-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f378-107">Der Status der Aktion Revoke-Lizenzen für das Token Apple Volume Purchase Program ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="6f378-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="6f378-108">Erbt vom [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f378-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6f378-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6f378-109">Properties</span></span>
|<span data-ttu-id="6f378-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f378-110">Property</span></span>|<span data-ttu-id="6f378-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6f378-111">Type</span></span>|<span data-ttu-id="6f378-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f378-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f378-113">actionName</span><span class="sxs-lookup"><span data-stu-id="6f378-113">actionName</span></span>|<span data-ttu-id="6f378-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f378-114">String</span></span>|<span data-ttu-id="6f378-115">Aktionsname Inherited aus [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f378-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="6f378-116">actionState</span><span class="sxs-lookup"><span data-stu-id="6f378-116">actionState</span></span>|[<span data-ttu-id="6f378-117">actionState</span><span class="sxs-lookup"><span data-stu-id="6f378-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6f378-118">Status der Aktion Inherited aus [VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="6f378-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="6f378-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6f378-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6f378-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6f378-120">startDateTime</span></span>|<span data-ttu-id="6f378-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f378-121">DateTimeOffset</span></span>|<span data-ttu-id="6f378-122">Zeit, die die Aktion initiiert wurde, von [VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="6f378-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="6f378-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f378-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="6f378-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f378-124">DateTimeOffset</span></span>|<span data-ttu-id="6f378-125">Aktualisiert der Status der Aktion letzten Inherited [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6f378-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="6f378-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="6f378-126">totalLicensesCount</span></span>|<span data-ttu-id="6f378-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6f378-127">Int32</span></span>|<span data-ttu-id="6f378-128">Anzahl der Anzahl der Lizenzen, die widerrufen versucht.</span><span class="sxs-lookup"><span data-stu-id="6f378-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="6f378-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="6f378-129">failedLicensesCount</span></span>|<span data-ttu-id="6f378-130">Int32</span><span class="sxs-lookup"><span data-stu-id="6f378-130">Int32</span></span>|<span data-ttu-id="6f378-131">Anzahl der die Anzahl der Lizenzen, die nicht widerrufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6f378-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="6f378-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="6f378-132">actionFailureReason</span></span>|[<span data-ttu-id="6f378-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="6f378-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="6f378-134">Der Grund für das Revoke Lizenzen-Aktion fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="6f378-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="6f378-135">Mögliche Werte sind: `none`, `appleFailure`, `internalError`, `expiredVppToken` und `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="6f378-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f378-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6f378-136">Relationships</span></span>
<span data-ttu-id="6f378-137">Keine</span><span class="sxs-lookup"><span data-stu-id="6f378-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f378-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6f378-138">JSON Representation</span></span>
<span data-ttu-id="6f378-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6f378-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```




