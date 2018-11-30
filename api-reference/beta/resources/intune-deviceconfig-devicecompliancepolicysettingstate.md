---
title: deviceCompliancePolicySettingState-Ressourcentyp
description: Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.
ms.openlocfilehash: d73cbe591e30e465065e0c446c6d98d7232a049c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063450"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="ce2e7-103">deviceCompliancePolicySettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ce2e7-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="ce2e7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ce2e7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce2e7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ce2e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce2e7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ce2e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce2e7-107">Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="ce2e7-107">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="ce2e7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ce2e7-108">Properties</span></span>
|<span data-ttu-id="ce2e7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce2e7-109">Property</span></span>|<span data-ttu-id="ce2e7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ce2e7-110">Type</span></span>|<span data-ttu-id="ce2e7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce2e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce2e7-112">setting</span><span class="sxs-lookup"><span data-stu-id="ce2e7-112">setting</span></span>|<span data-ttu-id="ce2e7-113">String</span><span class="sxs-lookup"><span data-stu-id="ce2e7-113">String</span></span>|<span data-ttu-id="ce2e7-114">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="ce2e7-114">The setting that is being reported</span></span>|
|<span data-ttu-id="ce2e7-115">settingName</span><span class="sxs-lookup"><span data-stu-id="ce2e7-115">settingName</span></span>|<span data-ttu-id="ce2e7-116">String</span><span class="sxs-lookup"><span data-stu-id="ce2e7-116">String</span></span>|<span data-ttu-id="ce2e7-117">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="ce2e7-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="ce2e7-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ce2e7-118">instanceDisplayName</span></span>|<span data-ttu-id="ce2e7-119">String</span><span class="sxs-lookup"><span data-stu-id="ce2e7-119">String</span></span>|<span data-ttu-id="ce2e7-120">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="ce2e7-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="ce2e7-121">state</span><span class="sxs-lookup"><span data-stu-id="ce2e7-121">state</span></span>|[<span data-ttu-id="ce2e7-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ce2e7-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ce2e7-123">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="ce2e7-123">The compliance state of the setting.</span></span> <span data-ttu-id="ce2e7-124">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ce2e7-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ce2e7-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="ce2e7-125">errorCode</span></span>|<span data-ttu-id="ce2e7-126">Int64</span><span class="sxs-lookup"><span data-stu-id="ce2e7-126">Int64</span></span>|<span data-ttu-id="ce2e7-127">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="ce2e7-127">Error code for the setting</span></span>|
|<span data-ttu-id="ce2e7-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="ce2e7-128">errorDescription</span></span>|<span data-ttu-id="ce2e7-129">String</span><span class="sxs-lookup"><span data-stu-id="ce2e7-129">String</span></span>|<span data-ttu-id="ce2e7-130">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="ce2e7-130">Error description</span></span>|
|<span data-ttu-id="ce2e7-131">userId</span><span class="sxs-lookup"><span data-stu-id="ce2e7-131">userId</span></span>|<span data-ttu-id="ce2e7-132">String</span><span class="sxs-lookup"><span data-stu-id="ce2e7-132">String</span></span>|<span data-ttu-id="ce2e7-133">UserId</span><span class="sxs-lookup"><span data-stu-id="ce2e7-133">UserId</span></span>|
|<span data-ttu-id="ce2e7-134">userName</span><span class="sxs-lookup"><span data-stu-id="ce2e7-134">userName</span></span>|<span data-ttu-id="ce2e7-135">String</span><span class="sxs-lookup"><span data-stu-id="ce2e7-135">String</span></span>|<span data-ttu-id="ce2e7-136">UserName</span><span class="sxs-lookup"><span data-stu-id="ce2e7-136">UserName</span></span>|
|<span data-ttu-id="ce2e7-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="ce2e7-137">userEmail</span></span>|<span data-ttu-id="ce2e7-138">String</span><span class="sxs-lookup"><span data-stu-id="ce2e7-138">String</span></span>|<span data-ttu-id="ce2e7-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="ce2e7-139">UserEmail</span></span>|
|<span data-ttu-id="ce2e7-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ce2e7-140">userPrincipalName</span></span>|<span data-ttu-id="ce2e7-141">String</span><span class="sxs-lookup"><span data-stu-id="ce2e7-141">String</span></span>|<span data-ttu-id="ce2e7-142">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="ce2e7-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="ce2e7-143">sources</span><span class="sxs-lookup"><span data-stu-id="ce2e7-143">sources</span></span>|<span data-ttu-id="ce2e7-144">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ce2e7-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="ce2e7-145">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="ce2e7-145">Contributing policies</span></span>|
|<span data-ttu-id="ce2e7-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="ce2e7-146">currentValue</span></span>|<span data-ttu-id="ce2e7-147">String</span><span class="sxs-lookup"><span data-stu-id="ce2e7-147">String</span></span>|<span data-ttu-id="ce2e7-148">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="ce2e7-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce2e7-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ce2e7-149">Relationships</span></span>
<span data-ttu-id="ce2e7-150">Keine</span><span class="sxs-lookup"><span data-stu-id="ce2e7-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ce2e7-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ce2e7-151">JSON Representation</span></span>
<span data-ttu-id="ce2e7-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ce2e7-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```





