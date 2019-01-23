---
title: deviceConfigurationSettingState-Ressourcentyp
description: Status der Konfigurationseinstellungen für ein bestimmtes Gerät
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9355cdf0aab60208246fdae699cda78be65d62ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415187"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="cb7a6-103">deviceConfigurationSettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cb7a6-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="cb7a6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cb7a6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb7a6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb7a6-107">Status der Konfigurationseinstellungen für ein bestimmtes Gerät</span><span class="sxs-lookup"><span data-stu-id="cb7a6-107">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="cb7a6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cb7a6-108">Properties</span></span>
|<span data-ttu-id="cb7a6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb7a6-109">Property</span></span>|<span data-ttu-id="cb7a6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="cb7a6-110">Type</span></span>|<span data-ttu-id="cb7a6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb7a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb7a6-112">setting</span><span class="sxs-lookup"><span data-stu-id="cb7a6-112">setting</span></span>|<span data-ttu-id="cb7a6-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb7a6-113">String</span></span>|<span data-ttu-id="cb7a6-114">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="cb7a6-114">The setting that is being reported</span></span>|
|<span data-ttu-id="cb7a6-115">settingName</span><span class="sxs-lookup"><span data-stu-id="cb7a6-115">settingName</span></span>|<span data-ttu-id="cb7a6-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb7a6-116">String</span></span>|<span data-ttu-id="cb7a6-117">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="cb7a6-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="cb7a6-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="cb7a6-118">instanceDisplayName</span></span>|<span data-ttu-id="cb7a6-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb7a6-119">String</span></span>|<span data-ttu-id="cb7a6-120">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="cb7a6-121">state</span><span class="sxs-lookup"><span data-stu-id="cb7a6-121">state</span></span>|[<span data-ttu-id="cb7a6-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="cb7a6-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="cb7a6-123">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-123">The compliance state of the setting.</span></span> <span data-ttu-id="cb7a6-124">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="cb7a6-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="cb7a6-125">errorCode</span></span>|<span data-ttu-id="cb7a6-126">Int64</span><span class="sxs-lookup"><span data-stu-id="cb7a6-126">Int64</span></span>|<span data-ttu-id="cb7a6-127">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="cb7a6-127">Error code for the setting</span></span>|
|<span data-ttu-id="cb7a6-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="cb7a6-128">errorDescription</span></span>|<span data-ttu-id="cb7a6-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb7a6-129">String</span></span>|<span data-ttu-id="cb7a6-130">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="cb7a6-130">Error description</span></span>|
|<span data-ttu-id="cb7a6-131">userId</span><span class="sxs-lookup"><span data-stu-id="cb7a6-131">userId</span></span>|<span data-ttu-id="cb7a6-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb7a6-132">String</span></span>|<span data-ttu-id="cb7a6-133">UserId</span><span class="sxs-lookup"><span data-stu-id="cb7a6-133">UserId</span></span>|
|<span data-ttu-id="cb7a6-134">userName</span><span class="sxs-lookup"><span data-stu-id="cb7a6-134">userName</span></span>|<span data-ttu-id="cb7a6-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb7a6-135">String</span></span>|<span data-ttu-id="cb7a6-136">UserName</span><span class="sxs-lookup"><span data-stu-id="cb7a6-136">UserName</span></span>|
|<span data-ttu-id="cb7a6-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="cb7a6-137">userEmail</span></span>|<span data-ttu-id="cb7a6-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb7a6-138">String</span></span>|<span data-ttu-id="cb7a6-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="cb7a6-139">UserEmail</span></span>|
|<span data-ttu-id="cb7a6-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cb7a6-140">userPrincipalName</span></span>|<span data-ttu-id="cb7a6-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb7a6-141">String</span></span>|<span data-ttu-id="cb7a6-142">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="cb7a6-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="cb7a6-143">sources</span><span class="sxs-lookup"><span data-stu-id="cb7a6-143">sources</span></span>|<span data-ttu-id="cb7a6-144">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cb7a6-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="cb7a6-145">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="cb7a6-145">Contributing policies</span></span>|
|<span data-ttu-id="cb7a6-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="cb7a6-146">currentValue</span></span>|<span data-ttu-id="cb7a6-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb7a6-147">String</span></span>|<span data-ttu-id="cb7a6-148">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="cb7a6-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb7a6-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cb7a6-149">Relationships</span></span>
<span data-ttu-id="cb7a6-150">Keine</span><span class="sxs-lookup"><span data-stu-id="cb7a6-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb7a6-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cb7a6-151">JSON Representation</span></span>
<span data-ttu-id="cb7a6-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
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




