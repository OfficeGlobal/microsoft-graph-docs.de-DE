---
title: deviceConfigurationSettingState-Ressourcentyp
description: Status der Konfigurationseinstellungen für ein bestimmtes Gerät
author: tfitzmac
ms.openlocfilehash: 545cb9bf0be410a5e9a0e25dbc242399c6dbc61f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320643"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="19977-103">deviceConfigurationSettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="19977-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="19977-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="19977-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19977-105">Status der Konfigurationseinstellungen für ein bestimmtes Gerät</span><span class="sxs-lookup"><span data-stu-id="19977-105">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="19977-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="19977-106">Properties</span></span>
|<span data-ttu-id="19977-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19977-107">Property</span></span>|<span data-ttu-id="19977-108">Typ</span><span class="sxs-lookup"><span data-stu-id="19977-108">Type</span></span>|<span data-ttu-id="19977-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19977-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19977-110">setting</span><span class="sxs-lookup"><span data-stu-id="19977-110">setting</span></span>|<span data-ttu-id="19977-111">String</span><span class="sxs-lookup"><span data-stu-id="19977-111">String</span></span>|<span data-ttu-id="19977-112">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="19977-112">The setting that is being reported</span></span>|
|<span data-ttu-id="19977-113">settingName</span><span class="sxs-lookup"><span data-stu-id="19977-113">settingName</span></span>|<span data-ttu-id="19977-114">String</span><span class="sxs-lookup"><span data-stu-id="19977-114">String</span></span>|<span data-ttu-id="19977-115">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="19977-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="19977-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="19977-116">instanceDisplayName</span></span>|<span data-ttu-id="19977-117">String</span><span class="sxs-lookup"><span data-stu-id="19977-117">String</span></span>|<span data-ttu-id="19977-118">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="19977-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="19977-119">state</span><span class="sxs-lookup"><span data-stu-id="19977-119">state</span></span>|[<span data-ttu-id="19977-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="19977-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="19977-121">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="19977-121">The compliance state of the setting.</span></span> <span data-ttu-id="19977-122">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="19977-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="19977-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="19977-123">errorCode</span></span>|<span data-ttu-id="19977-124">Int64</span><span class="sxs-lookup"><span data-stu-id="19977-124">Int64</span></span>|<span data-ttu-id="19977-125">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="19977-125">Error code for the setting</span></span>|
|<span data-ttu-id="19977-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="19977-126">errorDescription</span></span>|<span data-ttu-id="19977-127">String</span><span class="sxs-lookup"><span data-stu-id="19977-127">String</span></span>|<span data-ttu-id="19977-128">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="19977-128">Error description</span></span>|
|<span data-ttu-id="19977-129">userId</span><span class="sxs-lookup"><span data-stu-id="19977-129">userId</span></span>|<span data-ttu-id="19977-130">String</span><span class="sxs-lookup"><span data-stu-id="19977-130">String</span></span>|<span data-ttu-id="19977-131">UserId</span><span class="sxs-lookup"><span data-stu-id="19977-131">UserId</span></span>|
|<span data-ttu-id="19977-132">userName</span><span class="sxs-lookup"><span data-stu-id="19977-132">userName</span></span>|<span data-ttu-id="19977-133">String</span><span class="sxs-lookup"><span data-stu-id="19977-133">String</span></span>|<span data-ttu-id="19977-134">UserName</span><span class="sxs-lookup"><span data-stu-id="19977-134">UserName</span></span>|
|<span data-ttu-id="19977-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="19977-135">userEmail</span></span>|<span data-ttu-id="19977-136">String</span><span class="sxs-lookup"><span data-stu-id="19977-136">String</span></span>|<span data-ttu-id="19977-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="19977-137">UserEmail</span></span>|
|<span data-ttu-id="19977-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19977-138">userPrincipalName</span></span>|<span data-ttu-id="19977-139">String</span><span class="sxs-lookup"><span data-stu-id="19977-139">String</span></span>|<span data-ttu-id="19977-140">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="19977-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="19977-141">sources</span><span class="sxs-lookup"><span data-stu-id="19977-141">sources</span></span>|<span data-ttu-id="19977-142">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="19977-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="19977-143">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="19977-143">Contributing policies</span></span>|
|<span data-ttu-id="19977-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="19977-144">currentValue</span></span>|<span data-ttu-id="19977-145">String</span><span class="sxs-lookup"><span data-stu-id="19977-145">String</span></span>|<span data-ttu-id="19977-146">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="19977-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="19977-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="19977-147">Relationships</span></span>
<span data-ttu-id="19977-148">Keine</span><span class="sxs-lookup"><span data-stu-id="19977-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19977-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="19977-149">JSON Representation</span></span>
<span data-ttu-id="19977-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="19977-150">Here is a JSON representation of the resource.</span></span>
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



