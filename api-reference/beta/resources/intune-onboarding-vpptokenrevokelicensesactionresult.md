---
title: vppTokenRevokeLicensesActionResult-Ressourcentyp
description: Der Status der Aktion REVOKE Licenses, die für das Apple Volume Purchase Program-Token ausgeführt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3ccf2bfd72ae9f6aeb85e3a7228faac09a8b2c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158170"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="da7e5-103">vppTokenRevokeLicensesActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="da7e5-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="da7e5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da7e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da7e5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="da7e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da7e5-106">Der Status der Aktion REVOKE Licenses, die für das Apple Volume Purchase Program-Token ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="da7e5-106">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="da7e5-107">Erbt von [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="da7e5-107">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="da7e5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="da7e5-108">Properties</span></span>
|<span data-ttu-id="da7e5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da7e5-109">Property</span></span>|<span data-ttu-id="da7e5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="da7e5-110">Type</span></span>|<span data-ttu-id="da7e5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da7e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da7e5-112">actionName</span><span class="sxs-lookup"><span data-stu-id="da7e5-112">actionName</span></span>|<span data-ttu-id="da7e5-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da7e5-113">String</span></span>|<span data-ttu-id="da7e5-114">Von [VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) geerbter Aktionsname</span><span class="sxs-lookup"><span data-stu-id="da7e5-114">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="da7e5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="da7e5-115">actionState</span></span>|[<span data-ttu-id="da7e5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="da7e5-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="da7e5-117">Status der von [VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="da7e5-117">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="da7e5-118">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="da7e5-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="da7e5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="da7e5-119">startDateTime</span></span>|<span data-ttu-id="da7e5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da7e5-120">DateTimeOffset</span></span>|<span data-ttu-id="da7e5-121">Zeitpunkt, zu dem die Aktion initiiert wurde, geerbt von [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="da7e5-121">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="da7e5-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="da7e5-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="da7e5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da7e5-123">DateTimeOffset</span></span>|<span data-ttu-id="da7e5-124">Zeitpunkt, zu dem der Aktionsstatus zuletzt aktualisiert wurde, geerbt von [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="da7e5-124">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="da7e5-125">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="da7e5-125">totalLicensesCount</span></span>|<span data-ttu-id="da7e5-126">Int32</span><span class="sxs-lookup"><span data-stu-id="da7e5-126">Int32</span></span>|<span data-ttu-id="da7e5-127">Die Anzahl der zu wider rufenden Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="da7e5-127">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="da7e5-128">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="da7e5-128">failedLicensesCount</span></span>|<span data-ttu-id="da7e5-129">Int32</span><span class="sxs-lookup"><span data-stu-id="da7e5-129">Int32</span></span>|<span data-ttu-id="da7e5-130">Die Anzahl der Lizenzen, die nicht widerrufen werden konnten.</span><span class="sxs-lookup"><span data-stu-id="da7e5-130">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="da7e5-131">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="da7e5-131">actionFailureReason</span></span>|[<span data-ttu-id="da7e5-132">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="da7e5-132">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="da7e5-133">Der Grund für den Fehlschlagen der Lizenz Widerruf.</span><span class="sxs-lookup"><span data-stu-id="da7e5-133">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="da7e5-134">Mögliche Werte: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="da7e5-134">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da7e5-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="da7e5-135">Relationships</span></span>
<span data-ttu-id="da7e5-136">Keine</span><span class="sxs-lookup"><span data-stu-id="da7e5-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da7e5-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="da7e5-137">JSON Representation</span></span>
<span data-ttu-id="da7e5-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="da7e5-138">Here is a JSON representation of the resource.</span></span>
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




