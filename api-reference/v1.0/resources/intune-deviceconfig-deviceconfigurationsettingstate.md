---
title: deviceConfigurationSettingState-Ressourcentyp
description: Status der Konfigurationseinstellungen für ein bestimmtes Gerät
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: beed55d68c3ef7005a307d75fc1ee58ea78ed8d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845843"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="a9a94-103">deviceConfigurationSettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a9a94-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="a9a94-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a9a94-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9a94-105">Status der Konfigurationseinstellungen für ein bestimmtes Gerät</span><span class="sxs-lookup"><span data-stu-id="a9a94-105">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="a9a94-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a9a94-106">Properties</span></span>
|<span data-ttu-id="a9a94-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a9a94-107">Property</span></span>|<span data-ttu-id="a9a94-108">Typ</span><span class="sxs-lookup"><span data-stu-id="a9a94-108">Type</span></span>|<span data-ttu-id="a9a94-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9a94-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9a94-110">setting</span><span class="sxs-lookup"><span data-stu-id="a9a94-110">setting</span></span>|<span data-ttu-id="a9a94-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9a94-111">String</span></span>|<span data-ttu-id="a9a94-112">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="a9a94-112">The setting that is being reported</span></span>|
|<span data-ttu-id="a9a94-113">settingName</span><span class="sxs-lookup"><span data-stu-id="a9a94-113">settingName</span></span>|<span data-ttu-id="a9a94-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9a94-114">String</span></span>|<span data-ttu-id="a9a94-115">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="a9a94-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="a9a94-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a9a94-116">instanceDisplayName</span></span>|<span data-ttu-id="a9a94-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9a94-117">String</span></span>|<span data-ttu-id="a9a94-118">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="a9a94-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="a9a94-119">state</span><span class="sxs-lookup"><span data-stu-id="a9a94-119">state</span></span>|[<span data-ttu-id="a9a94-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a9a94-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a9a94-121">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="a9a94-121">The compliance state of the setting.</span></span> <span data-ttu-id="a9a94-122">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a9a94-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a9a94-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="a9a94-123">errorCode</span></span>|<span data-ttu-id="a9a94-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a9a94-124">Int64</span></span>|<span data-ttu-id="a9a94-125">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="a9a94-125">Error code for the setting</span></span>|
|<span data-ttu-id="a9a94-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="a9a94-126">errorDescription</span></span>|<span data-ttu-id="a9a94-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9a94-127">String</span></span>|<span data-ttu-id="a9a94-128">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="a9a94-128">Error description</span></span>|
|<span data-ttu-id="a9a94-129">userId</span><span class="sxs-lookup"><span data-stu-id="a9a94-129">userId</span></span>|<span data-ttu-id="a9a94-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9a94-130">String</span></span>|<span data-ttu-id="a9a94-131">UserId</span><span class="sxs-lookup"><span data-stu-id="a9a94-131">UserId</span></span>|
|<span data-ttu-id="a9a94-132">userName</span><span class="sxs-lookup"><span data-stu-id="a9a94-132">userName</span></span>|<span data-ttu-id="a9a94-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9a94-133">String</span></span>|<span data-ttu-id="a9a94-134">UserName</span><span class="sxs-lookup"><span data-stu-id="a9a94-134">UserName</span></span>|
|<span data-ttu-id="a9a94-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="a9a94-135">userEmail</span></span>|<span data-ttu-id="a9a94-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9a94-136">String</span></span>|<span data-ttu-id="a9a94-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="a9a94-137">UserEmail</span></span>|
|<span data-ttu-id="a9a94-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9a94-138">userPrincipalName</span></span>|<span data-ttu-id="a9a94-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9a94-139">String</span></span>|<span data-ttu-id="a9a94-140">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="a9a94-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="a9a94-141">sources</span><span class="sxs-lookup"><span data-stu-id="a9a94-141">sources</span></span>|<span data-ttu-id="a9a94-142">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a9a94-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="a9a94-143">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="a9a94-143">Contributing policies</span></span>|
|<span data-ttu-id="a9a94-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="a9a94-144">currentValue</span></span>|<span data-ttu-id="a9a94-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9a94-145">String</span></span>|<span data-ttu-id="a9a94-146">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="a9a94-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9a94-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a9a94-147">Relationships</span></span>
<span data-ttu-id="a9a94-148">Keine</span><span class="sxs-lookup"><span data-stu-id="a9a94-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a9a94-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a9a94-149">JSON Representation</span></span>
<span data-ttu-id="a9a94-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a9a94-150">Here is a JSON representation of the resource.</span></span>
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



