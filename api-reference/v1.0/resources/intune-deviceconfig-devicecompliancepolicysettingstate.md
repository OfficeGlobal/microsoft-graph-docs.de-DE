---
title: deviceCompliancePolicySettingState-Ressourcentyp
description: Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4d291f84a8c4404ff5b4425680260997b6b452f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261747"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="b872e-103">deviceCompliancePolicySettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b872e-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="b872e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b872e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b872e-105">Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="b872e-105">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b872e-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b872e-106">Properties</span></span>
|<span data-ttu-id="b872e-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b872e-107">Property</span></span>|<span data-ttu-id="b872e-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b872e-108">Type</span></span>|<span data-ttu-id="b872e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b872e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b872e-110">setting</span><span class="sxs-lookup"><span data-stu-id="b872e-110">setting</span></span>|<span data-ttu-id="b872e-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b872e-111">String</span></span>|<span data-ttu-id="b872e-112">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="b872e-112">The setting that is being reported</span></span>|
|<span data-ttu-id="b872e-113">settingName</span><span class="sxs-lookup"><span data-stu-id="b872e-113">settingName</span></span>|<span data-ttu-id="b872e-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b872e-114">String</span></span>|<span data-ttu-id="b872e-115">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="b872e-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="b872e-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b872e-116">instanceDisplayName</span></span>|<span data-ttu-id="b872e-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b872e-117">String</span></span>|<span data-ttu-id="b872e-118">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="b872e-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="b872e-119">state</span><span class="sxs-lookup"><span data-stu-id="b872e-119">state</span></span>|[<span data-ttu-id="b872e-120">Wurde</span><span class="sxs-lookup"><span data-stu-id="b872e-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b872e-121">Der Kompatibilitätsstatus der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="b872e-121">The compliance state of the setting.</span></span> <span data-ttu-id="b872e-122">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b872e-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b872e-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="b872e-123">errorCode</span></span>|<span data-ttu-id="b872e-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b872e-124">Int64</span></span>|<span data-ttu-id="b872e-125">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="b872e-125">Error code for the setting</span></span>|
|<span data-ttu-id="b872e-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b872e-126">errorDescription</span></span>|<span data-ttu-id="b872e-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b872e-127">String</span></span>|<span data-ttu-id="b872e-128">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="b872e-128">Error description</span></span>|
|<span data-ttu-id="b872e-129">userId</span><span class="sxs-lookup"><span data-stu-id="b872e-129">userId</span></span>|<span data-ttu-id="b872e-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b872e-130">String</span></span>|<span data-ttu-id="b872e-131">UserId</span><span class="sxs-lookup"><span data-stu-id="b872e-131">UserId</span></span>|
|<span data-ttu-id="b872e-132">userName</span><span class="sxs-lookup"><span data-stu-id="b872e-132">userName</span></span>|<span data-ttu-id="b872e-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b872e-133">String</span></span>|<span data-ttu-id="b872e-134">UserName</span><span class="sxs-lookup"><span data-stu-id="b872e-134">UserName</span></span>|
|<span data-ttu-id="b872e-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="b872e-135">userEmail</span></span>|<span data-ttu-id="b872e-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b872e-136">String</span></span>|<span data-ttu-id="b872e-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="b872e-137">UserEmail</span></span>|
|<span data-ttu-id="b872e-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b872e-138">userPrincipalName</span></span>|<span data-ttu-id="b872e-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b872e-139">String</span></span>|<span data-ttu-id="b872e-140">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="b872e-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="b872e-141">sources</span><span class="sxs-lookup"><span data-stu-id="b872e-141">sources</span></span>|<span data-ttu-id="b872e-142">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b872e-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b872e-143">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="b872e-143">Contributing policies</span></span>|
|<span data-ttu-id="b872e-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="b872e-144">currentValue</span></span>|<span data-ttu-id="b872e-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b872e-145">String</span></span>|<span data-ttu-id="b872e-146">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="b872e-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b872e-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b872e-147">Relationships</span></span>
<span data-ttu-id="b872e-148">Keine</span><span class="sxs-lookup"><span data-stu-id="b872e-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b872e-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b872e-149">JSON Representation</span></span>
<span data-ttu-id="b872e-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b872e-150">Here is a JSON representation of the resource.</span></span>
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



