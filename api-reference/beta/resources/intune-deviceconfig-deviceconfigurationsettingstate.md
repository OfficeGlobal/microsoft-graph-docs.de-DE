---
title: deviceConfigurationSettingState-Ressourcentyp
description: Status der Konfigurationseinstellungen für ein bestimmtes Gerät
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 25d4d8d35467227660bb6a5fe3550077377be979
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885729"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="38723-103">deviceConfigurationSettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="38723-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="38723-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="38723-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38723-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="38723-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38723-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="38723-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38723-107">Status der Konfigurationseinstellungen für ein bestimmtes Gerät</span><span class="sxs-lookup"><span data-stu-id="38723-107">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="38723-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="38723-108">Properties</span></span>
|<span data-ttu-id="38723-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38723-109">Property</span></span>|<span data-ttu-id="38723-110">Typ</span><span class="sxs-lookup"><span data-stu-id="38723-110">Type</span></span>|<span data-ttu-id="38723-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38723-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38723-112">setting</span><span class="sxs-lookup"><span data-stu-id="38723-112">setting</span></span>|<span data-ttu-id="38723-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38723-113">String</span></span>|<span data-ttu-id="38723-114">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="38723-114">The setting that is being reported</span></span>|
|<span data-ttu-id="38723-115">settingName</span><span class="sxs-lookup"><span data-stu-id="38723-115">settingName</span></span>|<span data-ttu-id="38723-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38723-116">String</span></span>|<span data-ttu-id="38723-117">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="38723-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="38723-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="38723-118">instanceDisplayName</span></span>|<span data-ttu-id="38723-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38723-119">String</span></span>|<span data-ttu-id="38723-120">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="38723-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="38723-121">state</span><span class="sxs-lookup"><span data-stu-id="38723-121">state</span></span>|[<span data-ttu-id="38723-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="38723-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="38723-123">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="38723-123">The compliance state of the setting.</span></span> <span data-ttu-id="38723-124">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="38723-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="38723-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="38723-125">errorCode</span></span>|<span data-ttu-id="38723-126">Int64</span><span class="sxs-lookup"><span data-stu-id="38723-126">Int64</span></span>|<span data-ttu-id="38723-127">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="38723-127">Error code for the setting</span></span>|
|<span data-ttu-id="38723-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="38723-128">errorDescription</span></span>|<span data-ttu-id="38723-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38723-129">String</span></span>|<span data-ttu-id="38723-130">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="38723-130">Error description</span></span>|
|<span data-ttu-id="38723-131">userId</span><span class="sxs-lookup"><span data-stu-id="38723-131">userId</span></span>|<span data-ttu-id="38723-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38723-132">String</span></span>|<span data-ttu-id="38723-133">UserId</span><span class="sxs-lookup"><span data-stu-id="38723-133">UserId</span></span>|
|<span data-ttu-id="38723-134">userName</span><span class="sxs-lookup"><span data-stu-id="38723-134">userName</span></span>|<span data-ttu-id="38723-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38723-135">String</span></span>|<span data-ttu-id="38723-136">UserName</span><span class="sxs-lookup"><span data-stu-id="38723-136">UserName</span></span>|
|<span data-ttu-id="38723-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="38723-137">userEmail</span></span>|<span data-ttu-id="38723-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38723-138">String</span></span>|<span data-ttu-id="38723-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="38723-139">UserEmail</span></span>|
|<span data-ttu-id="38723-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="38723-140">userPrincipalName</span></span>|<span data-ttu-id="38723-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38723-141">String</span></span>|<span data-ttu-id="38723-142">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="38723-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="38723-143">sources</span><span class="sxs-lookup"><span data-stu-id="38723-143">sources</span></span>|<span data-ttu-id="38723-144">[settingSource](../resources/intune-deviceconfig-settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="38723-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="38723-145">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="38723-145">Contributing policies</span></span>|
|<span data-ttu-id="38723-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="38723-146">currentValue</span></span>|<span data-ttu-id="38723-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38723-147">String</span></span>|<span data-ttu-id="38723-148">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="38723-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="38723-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="38723-149">Relationships</span></span>
<span data-ttu-id="38723-150">Keine</span><span class="sxs-lookup"><span data-stu-id="38723-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="38723-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="38723-151">JSON Representation</span></span>
<span data-ttu-id="38723-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="38723-152">Here is a JSON representation of the resource.</span></span>
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





