---
title: deviceCompliancePolicySettingState-Ressourcentyp
description: Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b17930161f66ca83d59e3f2f62777a79f82b79f0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425736"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="9483d-103">deviceCompliancePolicySettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9483d-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="9483d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9483d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9483d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9483d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9483d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9483d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9483d-107">Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="9483d-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="9483d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9483d-108">Properties</span></span>
|<span data-ttu-id="9483d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9483d-109">Property</span></span>|<span data-ttu-id="9483d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9483d-110">Type</span></span>|<span data-ttu-id="9483d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9483d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9483d-112">setting</span><span class="sxs-lookup"><span data-stu-id="9483d-112">setting</span></span>|<span data-ttu-id="9483d-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9483d-113">String</span></span>|<span data-ttu-id="9483d-114">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="9483d-114">The setting that is being reported</span></span>|
|<span data-ttu-id="9483d-115">settingName</span><span class="sxs-lookup"><span data-stu-id="9483d-115">settingName</span></span>|<span data-ttu-id="9483d-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9483d-116">String</span></span>|<span data-ttu-id="9483d-117">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="9483d-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="9483d-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9483d-118">instanceDisplayName</span></span>|<span data-ttu-id="9483d-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9483d-119">String</span></span>|<span data-ttu-id="9483d-120">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="9483d-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="9483d-121">state</span><span class="sxs-lookup"><span data-stu-id="9483d-121">state</span></span>|[<span data-ttu-id="9483d-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9483d-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9483d-123">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="9483d-123">The compliance state of the setting.</span></span> <span data-ttu-id="9483d-124">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="9483d-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9483d-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="9483d-125">errorCode</span></span>|<span data-ttu-id="9483d-126">Int64</span><span class="sxs-lookup"><span data-stu-id="9483d-126">Int64</span></span>|<span data-ttu-id="9483d-127">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="9483d-127">Error code for the setting</span></span>|
|<span data-ttu-id="9483d-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="9483d-128">errorDescription</span></span>|<span data-ttu-id="9483d-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9483d-129">String</span></span>|<span data-ttu-id="9483d-130">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="9483d-130">Error description</span></span>|
|<span data-ttu-id="9483d-131">userId</span><span class="sxs-lookup"><span data-stu-id="9483d-131">userId</span></span>|<span data-ttu-id="9483d-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9483d-132">String</span></span>|<span data-ttu-id="9483d-133">UserId</span><span class="sxs-lookup"><span data-stu-id="9483d-133">UserId</span></span>|
|<span data-ttu-id="9483d-134">userName</span><span class="sxs-lookup"><span data-stu-id="9483d-134">userName</span></span>|<span data-ttu-id="9483d-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9483d-135">String</span></span>|<span data-ttu-id="9483d-136">UserName</span><span class="sxs-lookup"><span data-stu-id="9483d-136">UserName</span></span>|
|<span data-ttu-id="9483d-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="9483d-137">userEmail</span></span>|<span data-ttu-id="9483d-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9483d-138">String</span></span>|<span data-ttu-id="9483d-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="9483d-139">UserEmail</span></span>|
|<span data-ttu-id="9483d-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9483d-140">userPrincipalName</span></span>|<span data-ttu-id="9483d-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9483d-141">String</span></span>|<span data-ttu-id="9483d-142">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="9483d-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="9483d-143">sources</span><span class="sxs-lookup"><span data-stu-id="9483d-143">sources</span></span>|<span data-ttu-id="9483d-144">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9483d-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="9483d-145">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="9483d-145">Contributing policies</span></span>|
|<span data-ttu-id="9483d-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="9483d-146">currentValue</span></span>|<span data-ttu-id="9483d-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9483d-147">String</span></span>|<span data-ttu-id="9483d-148">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="9483d-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="9483d-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9483d-149">Relationships</span></span>
<span data-ttu-id="9483d-150">Keine</span><span class="sxs-lookup"><span data-stu-id="9483d-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9483d-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9483d-151">JSON Representation</span></span>
<span data-ttu-id="9483d-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9483d-152">Here is a JSON representation of the resource.</span></span>
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




