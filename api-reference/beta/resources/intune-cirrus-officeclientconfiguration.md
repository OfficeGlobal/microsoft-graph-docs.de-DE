---
title: Ressourcentyp officeClientConfiguration
description: Office-Client-Konfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c171f5f9f3dcedcab0d14b98a6fea0ba8fbe41eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393235"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="bb43a-103">Ressourcentyp officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb43a-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="bb43a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bb43a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb43a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bb43a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb43a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bb43a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb43a-107">Office-Client-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="bb43a-107">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="bb43a-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="bb43a-108">Methods</span></span>
|<span data-ttu-id="bb43a-109">Methode</span><span class="sxs-lookup"><span data-stu-id="bb43a-109">Method</span></span>|<span data-ttu-id="bb43a-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bb43a-110">Return Type</span></span>|<span data-ttu-id="bb43a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb43a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb43a-112">Liste officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="bb43a-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="bb43a-113">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bb43a-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="bb43a-114">Listeneigenschaften und Beziehungen der [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="bb43a-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="bb43a-115">Abrufen von officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb43a-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="bb43a-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb43a-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="bb43a-117">Lesen Sie Eigenschaften und Beziehungen des [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb43a-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bb43a-118">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="bb43a-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="bb43a-119">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bb43a-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bb43a-120">Ersetzen Sie alle Gruppen für eine Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="bb43a-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="bb43a-121">UpdatePriorities Aktion</span><span class="sxs-lookup"><span data-stu-id="bb43a-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="bb43a-122">Keine</span><span class="sxs-lookup"><span data-stu-id="bb43a-122">None</span></span>|<span data-ttu-id="bb43a-123">Aktualisieren Sie die Richtlinie Prioritäten.</span><span class="sxs-lookup"><span data-stu-id="bb43a-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb43a-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb43a-124">Properties</span></span>
|<span data-ttu-id="bb43a-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb43a-125">Property</span></span>|<span data-ttu-id="bb43a-126">Typ</span><span class="sxs-lookup"><span data-stu-id="bb43a-126">Type</span></span>|<span data-ttu-id="bb43a-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb43a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb43a-128">id</span><span class="sxs-lookup"><span data-stu-id="bb43a-128">id</span></span>|<span data-ttu-id="bb43a-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb43a-129">String</span></span>|<span data-ttu-id="bb43a-130">ID des die Richtlinie Office-Client-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="bb43a-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="bb43a-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="bb43a-131">userPreferencePayload</span></span>|<span data-ttu-id="bb43a-132">Stream</span><span class="sxs-lookup"><span data-stu-id="bb43a-132">Stream</span></span>|<span data-ttu-id="bb43a-133">Vorgaben JSON-Zeichenfolge im Binärformat, können diese Werte vom Benutzer außer Kraft gesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="bb43a-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="bb43a-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="bb43a-134">policyPayload</span></span>|<span data-ttu-id="bb43a-135">Stream</span><span class="sxs-lookup"><span data-stu-id="bb43a-135">Stream</span></span>|<span data-ttu-id="bb43a-136">Richtlinieneinstellungen für JSON-Zeichenfolge im Binärformat, diese Werte können nicht vom Benutzer geändert werden.</span><span class="sxs-lookup"><span data-stu-id="bb43a-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="bb43a-137">description</span><span class="sxs-lookup"><span data-stu-id="bb43a-137">description</span></span>|<span data-ttu-id="bb43a-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb43a-138">String</span></span>|<span data-ttu-id="bb43a-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bb43a-139">Not yet documented</span></span>|
|<span data-ttu-id="bb43a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="bb43a-140">displayName</span></span>|<span data-ttu-id="bb43a-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb43a-141">String</span></span>|<span data-ttu-id="bb43a-142">Admin bereitgestellte Beschreibung für den Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="bb43a-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="bb43a-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb43a-143">lastModifiedDateTime</span></span>|<span data-ttu-id="bb43a-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="bb43a-144">DateTime</span></span>|<span data-ttu-id="bb43a-145">Zuletzt geänderte Datetime-Stempel der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="bb43a-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="bb43a-146">Priorität</span><span class="sxs-lookup"><span data-stu-id="bb43a-146">priority</span></span>|<span data-ttu-id="bb43a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bb43a-147">Int32</span></span>|<span data-ttu-id="bb43a-148">Prioritätswert sollte eindeutigen Wert für jede Richtlinie unter einem Mandanten sein und für konfliktlösung verwendet werden, niedrigere Werte bedeuten, dass Priorität hoch ist.</span><span class="sxs-lookup"><span data-stu-id="bb43a-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="bb43a-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bb43a-149">userCheckinSummary</span></span>|[<span data-ttu-id="bb43a-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bb43a-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="bb43a-151">Benutzer Einchecken Zusammenfassung für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="bb43a-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="bb43a-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="bb43a-152">checkinStatuses</span></span>|<span data-ttu-id="bb43a-153">[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bb43a-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="bb43a-154">Liste der Office-Client Einchecken Status.</span><span class="sxs-lookup"><span data-stu-id="bb43a-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb43a-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bb43a-155">Relationships</span></span>
|<span data-ttu-id="bb43a-156">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bb43a-156">Relationship</span></span>|<span data-ttu-id="bb43a-157">Typ</span><span class="sxs-lookup"><span data-stu-id="bb43a-157">Type</span></span>|<span data-ttu-id="bb43a-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb43a-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb43a-159">assignments</span><span class="sxs-lookup"><span data-stu-id="bb43a-159">assignments</span></span>|<span data-ttu-id="bb43a-160">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bb43a-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bb43a-161">Die Liste der zugewiesenen Gruppe für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="bb43a-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb43a-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bb43a-162">JSON Representation</span></span>
<span data-ttu-id="bb43a-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bb43a-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```



