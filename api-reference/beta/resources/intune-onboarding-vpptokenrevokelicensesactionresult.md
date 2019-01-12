---
title: Ressourcentyp vppTokenRevokeLicensesActionResult
description: Der Status der Aktion Revoke-Lizenzen für das Token Apple Volume Purchase Program ausgeführt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7044c07b4cc38168219d205f788f4eb8e3eafcf4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928815"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="d6c99-103">Ressourcentyp vppTokenRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="d6c99-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="d6c99-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d6c99-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6c99-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d6c99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6c99-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d6c99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6c99-107">Der Status der Aktion Revoke-Lizenzen für das Token Apple Volume Purchase Program ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="d6c99-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>

<span data-ttu-id="d6c99-108">Erbt vom [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d6c99-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6c99-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d6c99-109">Properties</span></span>
|<span data-ttu-id="d6c99-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d6c99-110">Property</span></span>|<span data-ttu-id="d6c99-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d6c99-111">Type</span></span>|<span data-ttu-id="d6c99-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6c99-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6c99-113">actionName</span><span class="sxs-lookup"><span data-stu-id="d6c99-113">actionName</span></span>|<span data-ttu-id="d6c99-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d6c99-114">String</span></span>|<span data-ttu-id="d6c99-115">Aktionsname Inherited aus [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d6c99-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="d6c99-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d6c99-116">actionState</span></span>|[<span data-ttu-id="d6c99-117">actionState</span><span class="sxs-lookup"><span data-stu-id="d6c99-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d6c99-118">Status der Aktion Inherited aus [VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d6c99-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="d6c99-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d6c99-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d6c99-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d6c99-120">startDateTime</span></span>|<span data-ttu-id="d6c99-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6c99-121">DateTimeOffset</span></span>|<span data-ttu-id="d6c99-122">Zeit, die die Aktion initiiert wurde, von [VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="d6c99-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="d6c99-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6c99-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="d6c99-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6c99-124">DateTimeOffset</span></span>|<span data-ttu-id="d6c99-125">Aktualisiert der Status der Aktion letzten Inherited [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d6c99-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="d6c99-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="d6c99-126">totalLicensesCount</span></span>|<span data-ttu-id="d6c99-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d6c99-127">Int32</span></span>|<span data-ttu-id="d6c99-128">Anzahl der Anzahl der Lizenzen, die widerrufen versucht.</span><span class="sxs-lookup"><span data-stu-id="d6c99-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="d6c99-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="d6c99-129">failedLicensesCount</span></span>|<span data-ttu-id="d6c99-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d6c99-130">Int32</span></span>|<span data-ttu-id="d6c99-131">Anzahl der die Anzahl der Lizenzen, die nicht widerrufen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d6c99-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="d6c99-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="d6c99-132">actionFailureReason</span></span>|[<span data-ttu-id="d6c99-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="d6c99-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="d6c99-134">Der Grund für das Revoke Lizenzen-Aktion fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="d6c99-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="d6c99-135">Mögliche Werte sind: `none`, `appleFailure`, `internalError`, `expiredVppToken` und `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="d6c99-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6c99-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d6c99-136">Relationships</span></span>
<span data-ttu-id="d6c99-137">Keine</span><span class="sxs-lookup"><span data-stu-id="d6c99-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6c99-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d6c99-138">JSON Representation</span></span>
<span data-ttu-id="d6c99-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d6c99-139">Here is a JSON representation of the resource.</span></span>
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





