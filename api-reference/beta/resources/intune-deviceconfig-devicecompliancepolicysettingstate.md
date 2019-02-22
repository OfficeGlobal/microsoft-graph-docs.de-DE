---
title: deviceCompliancePolicySettingState-Ressourcentyp
description: Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0b98cc4809fb72bb7caf5fe55fe6e912fd00f9b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171498"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="7697c-103">deviceCompliancePolicySettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7697c-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="7697c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7697c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7697c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7697c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7697c-106">Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="7697c-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="7697c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7697c-107">Properties</span></span>
|<span data-ttu-id="7697c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7697c-108">Property</span></span>|<span data-ttu-id="7697c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="7697c-109">Type</span></span>|<span data-ttu-id="7697c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7697c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7697c-111">setting</span><span class="sxs-lookup"><span data-stu-id="7697c-111">setting</span></span>|<span data-ttu-id="7697c-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7697c-112">String</span></span>|<span data-ttu-id="7697c-113">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="7697c-113">The setting that is being reported</span></span>|
|<span data-ttu-id="7697c-114">settingName</span><span class="sxs-lookup"><span data-stu-id="7697c-114">settingName</span></span>|<span data-ttu-id="7697c-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7697c-115">String</span></span>|<span data-ttu-id="7697c-116">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="7697c-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="7697c-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7697c-117">instanceDisplayName</span></span>|<span data-ttu-id="7697c-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7697c-118">String</span></span>|<span data-ttu-id="7697c-119">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="7697c-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="7697c-120">state</span><span class="sxs-lookup"><span data-stu-id="7697c-120">state</span></span>|[<span data-ttu-id="7697c-121">Wurde</span><span class="sxs-lookup"><span data-stu-id="7697c-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7697c-122">Der Kompatibilitätsstatus der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="7697c-122">The compliance state of the setting.</span></span> <span data-ttu-id="7697c-123">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="7697c-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7697c-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="7697c-124">errorCode</span></span>|<span data-ttu-id="7697c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="7697c-125">Int64</span></span>|<span data-ttu-id="7697c-126">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="7697c-126">Error code for the setting</span></span>|
|<span data-ttu-id="7697c-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="7697c-127">errorDescription</span></span>|<span data-ttu-id="7697c-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7697c-128">String</span></span>|<span data-ttu-id="7697c-129">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="7697c-129">Error description</span></span>|
|<span data-ttu-id="7697c-130">userId</span><span class="sxs-lookup"><span data-stu-id="7697c-130">userId</span></span>|<span data-ttu-id="7697c-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7697c-131">String</span></span>|<span data-ttu-id="7697c-132">UserId</span><span class="sxs-lookup"><span data-stu-id="7697c-132">UserId</span></span>|
|<span data-ttu-id="7697c-133">userName</span><span class="sxs-lookup"><span data-stu-id="7697c-133">userName</span></span>|<span data-ttu-id="7697c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7697c-134">String</span></span>|<span data-ttu-id="7697c-135">UserName</span><span class="sxs-lookup"><span data-stu-id="7697c-135">UserName</span></span>|
|<span data-ttu-id="7697c-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="7697c-136">userEmail</span></span>|<span data-ttu-id="7697c-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7697c-137">String</span></span>|<span data-ttu-id="7697c-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="7697c-138">UserEmail</span></span>|
|<span data-ttu-id="7697c-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7697c-139">userPrincipalName</span></span>|<span data-ttu-id="7697c-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7697c-140">String</span></span>|<span data-ttu-id="7697c-141">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="7697c-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="7697c-142">sources</span><span class="sxs-lookup"><span data-stu-id="7697c-142">sources</span></span>|<span data-ttu-id="7697c-143">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7697c-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="7697c-144">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="7697c-144">Contributing policies</span></span>|
|<span data-ttu-id="7697c-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="7697c-145">currentValue</span></span>|<span data-ttu-id="7697c-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7697c-146">String</span></span>|<span data-ttu-id="7697c-147">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="7697c-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="7697c-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7697c-148">Relationships</span></span>
<span data-ttu-id="7697c-149">Keine</span><span class="sxs-lookup"><span data-stu-id="7697c-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7697c-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7697c-150">JSON Representation</span></span>
<span data-ttu-id="7697c-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7697c-151">Here is a JSON representation of the resource.</span></span>
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




