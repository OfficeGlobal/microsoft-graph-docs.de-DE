---
title: deviceConfigurationSettingState-Ressourcentyp
description: Status der Konfigurationseinstellungen für ein bestimmtes Gerät
ms.openlocfilehash: 551b5ccb215492f48d9cd26bcf8b7e2cb80ed787
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061595"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="264e2-103">deviceConfigurationSettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="264e2-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="264e2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="264e2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="264e2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="264e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="264e2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="264e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="264e2-107">Status der Konfigurationseinstellungen für ein bestimmtes Gerät</span><span class="sxs-lookup"><span data-stu-id="264e2-107">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="264e2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="264e2-108">Properties</span></span>
|<span data-ttu-id="264e2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="264e2-109">Property</span></span>|<span data-ttu-id="264e2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="264e2-110">Type</span></span>|<span data-ttu-id="264e2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="264e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="264e2-112">setting</span><span class="sxs-lookup"><span data-stu-id="264e2-112">setting</span></span>|<span data-ttu-id="264e2-113">String</span><span class="sxs-lookup"><span data-stu-id="264e2-113">String</span></span>|<span data-ttu-id="264e2-114">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="264e2-114">The setting that is being reported</span></span>|
|<span data-ttu-id="264e2-115">settingName</span><span class="sxs-lookup"><span data-stu-id="264e2-115">settingName</span></span>|<span data-ttu-id="264e2-116">String</span><span class="sxs-lookup"><span data-stu-id="264e2-116">String</span></span>|<span data-ttu-id="264e2-117">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="264e2-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="264e2-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="264e2-118">instanceDisplayName</span></span>|<span data-ttu-id="264e2-119">String</span><span class="sxs-lookup"><span data-stu-id="264e2-119">String</span></span>|<span data-ttu-id="264e2-120">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="264e2-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="264e2-121">state</span><span class="sxs-lookup"><span data-stu-id="264e2-121">state</span></span>|[<span data-ttu-id="264e2-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="264e2-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="264e2-123">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="264e2-123">The compliance state of the setting.</span></span> <span data-ttu-id="264e2-124">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="264e2-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="264e2-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="264e2-125">errorCode</span></span>|<span data-ttu-id="264e2-126">Int64</span><span class="sxs-lookup"><span data-stu-id="264e2-126">Int64</span></span>|<span data-ttu-id="264e2-127">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="264e2-127">Error code for the setting</span></span>|
|<span data-ttu-id="264e2-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="264e2-128">errorDescription</span></span>|<span data-ttu-id="264e2-129">String</span><span class="sxs-lookup"><span data-stu-id="264e2-129">String</span></span>|<span data-ttu-id="264e2-130">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="264e2-130">Error description</span></span>|
|<span data-ttu-id="264e2-131">userId</span><span class="sxs-lookup"><span data-stu-id="264e2-131">userId</span></span>|<span data-ttu-id="264e2-132">String</span><span class="sxs-lookup"><span data-stu-id="264e2-132">String</span></span>|<span data-ttu-id="264e2-133">UserId</span><span class="sxs-lookup"><span data-stu-id="264e2-133">UserId</span></span>|
|<span data-ttu-id="264e2-134">userName</span><span class="sxs-lookup"><span data-stu-id="264e2-134">userName</span></span>|<span data-ttu-id="264e2-135">String</span><span class="sxs-lookup"><span data-stu-id="264e2-135">String</span></span>|<span data-ttu-id="264e2-136">UserName</span><span class="sxs-lookup"><span data-stu-id="264e2-136">UserName</span></span>|
|<span data-ttu-id="264e2-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="264e2-137">userEmail</span></span>|<span data-ttu-id="264e2-138">String</span><span class="sxs-lookup"><span data-stu-id="264e2-138">String</span></span>|<span data-ttu-id="264e2-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="264e2-139">UserEmail</span></span>|
|<span data-ttu-id="264e2-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="264e2-140">userPrincipalName</span></span>|<span data-ttu-id="264e2-141">String</span><span class="sxs-lookup"><span data-stu-id="264e2-141">String</span></span>|<span data-ttu-id="264e2-142">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="264e2-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="264e2-143">sources</span><span class="sxs-lookup"><span data-stu-id="264e2-143">sources</span></span>|<span data-ttu-id="264e2-144">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="264e2-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="264e2-145">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="264e2-145">Contributing policies</span></span>|
|<span data-ttu-id="264e2-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="264e2-146">currentValue</span></span>|<span data-ttu-id="264e2-147">String</span><span class="sxs-lookup"><span data-stu-id="264e2-147">String</span></span>|<span data-ttu-id="264e2-148">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="264e2-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="264e2-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="264e2-149">Relationships</span></span>
<span data-ttu-id="264e2-150">Keine</span><span class="sxs-lookup"><span data-stu-id="264e2-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="264e2-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="264e2-151">JSON Representation</span></span>
<span data-ttu-id="264e2-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="264e2-152">Here is a JSON representation of the resource.</span></span>
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





