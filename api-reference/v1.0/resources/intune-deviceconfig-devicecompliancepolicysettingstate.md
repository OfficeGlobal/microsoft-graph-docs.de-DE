---
title: deviceCompliancePolicySettingState-Ressourcentyp
description: Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 85de06b5baa9ff840ab0e1fd18cb70b0f5676e8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962212"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="c4b0b-103">deviceCompliancePolicySettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c4b0b-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="c4b0b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c4b0b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4b0b-105">Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="c4b0b-105">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="c4b0b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c4b0b-106">Properties</span></span>
|<span data-ttu-id="c4b0b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c4b0b-107">Property</span></span>|<span data-ttu-id="c4b0b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c4b0b-108">Type</span></span>|<span data-ttu-id="c4b0b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4b0b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4b0b-110">setting</span><span class="sxs-lookup"><span data-stu-id="c4b0b-110">setting</span></span>|<span data-ttu-id="c4b0b-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4b0b-111">String</span></span>|<span data-ttu-id="c4b0b-112">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="c4b0b-112">The setting that is being reported</span></span>|
|<span data-ttu-id="c4b0b-113">settingName</span><span class="sxs-lookup"><span data-stu-id="c4b0b-113">settingName</span></span>|<span data-ttu-id="c4b0b-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4b0b-114">String</span></span>|<span data-ttu-id="c4b0b-115">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="c4b0b-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="c4b0b-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c4b0b-116">instanceDisplayName</span></span>|<span data-ttu-id="c4b0b-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4b0b-117">String</span></span>|<span data-ttu-id="c4b0b-118">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="c4b0b-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="c4b0b-119">state</span><span class="sxs-lookup"><span data-stu-id="c4b0b-119">state</span></span>|[<span data-ttu-id="c4b0b-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c4b0b-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c4b0b-121">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="c4b0b-121">The compliance state of the setting.</span></span> <span data-ttu-id="c4b0b-122">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c4b0b-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c4b0b-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="c4b0b-123">errorCode</span></span>|<span data-ttu-id="c4b0b-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c4b0b-124">Int64</span></span>|<span data-ttu-id="c4b0b-125">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="c4b0b-125">Error code for the setting</span></span>|
|<span data-ttu-id="c4b0b-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="c4b0b-126">errorDescription</span></span>|<span data-ttu-id="c4b0b-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4b0b-127">String</span></span>|<span data-ttu-id="c4b0b-128">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="c4b0b-128">Error description</span></span>|
|<span data-ttu-id="c4b0b-129">userId</span><span class="sxs-lookup"><span data-stu-id="c4b0b-129">userId</span></span>|<span data-ttu-id="c4b0b-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4b0b-130">String</span></span>|<span data-ttu-id="c4b0b-131">UserId</span><span class="sxs-lookup"><span data-stu-id="c4b0b-131">UserId</span></span>|
|<span data-ttu-id="c4b0b-132">userName</span><span class="sxs-lookup"><span data-stu-id="c4b0b-132">userName</span></span>|<span data-ttu-id="c4b0b-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4b0b-133">String</span></span>|<span data-ttu-id="c4b0b-134">UserName</span><span class="sxs-lookup"><span data-stu-id="c4b0b-134">UserName</span></span>|
|<span data-ttu-id="c4b0b-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="c4b0b-135">userEmail</span></span>|<span data-ttu-id="c4b0b-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4b0b-136">String</span></span>|<span data-ttu-id="c4b0b-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="c4b0b-137">UserEmail</span></span>|
|<span data-ttu-id="c4b0b-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c4b0b-138">userPrincipalName</span></span>|<span data-ttu-id="c4b0b-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4b0b-139">String</span></span>|<span data-ttu-id="c4b0b-140">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="c4b0b-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="c4b0b-141">sources</span><span class="sxs-lookup"><span data-stu-id="c4b0b-141">sources</span></span>|<span data-ttu-id="c4b0b-142">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c4b0b-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="c4b0b-143">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="c4b0b-143">Contributing policies</span></span>|
|<span data-ttu-id="c4b0b-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="c4b0b-144">currentValue</span></span>|<span data-ttu-id="c4b0b-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4b0b-145">String</span></span>|<span data-ttu-id="c4b0b-146">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="c4b0b-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4b0b-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c4b0b-147">Relationships</span></span>
<span data-ttu-id="c4b0b-148">Keine</span><span class="sxs-lookup"><span data-stu-id="c4b0b-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4b0b-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c4b0b-149">JSON Representation</span></span>
<span data-ttu-id="c4b0b-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c4b0b-150">Here is a JSON representation of the resource.</span></span>
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



