---
title: Ressourcentyp officeClientConfiguration
description: Office-Client-Konfiguration.
author: tfitzmac
ms.openlocfilehash: 67a7845a2e0327e2e5de37d424274f6e2ee35604
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303836"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="11657-103">Ressourcentyp officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="11657-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="11657-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="11657-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11657-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="11657-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11657-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="11657-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11657-107">Office-Client-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="11657-107">Office Client Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="11657-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="11657-108">Methods</span></span>
|<span data-ttu-id="11657-109">Methode</span><span class="sxs-lookup"><span data-stu-id="11657-109">Method</span></span>|<span data-ttu-id="11657-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="11657-110">Return Type</span></span>|<span data-ttu-id="11657-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11657-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11657-112">Liste officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="11657-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="11657-113">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="11657-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="11657-114">Listeneigenschaften und Beziehungen der [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="11657-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="11657-115">Abrufen von officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="11657-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="11657-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="11657-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="11657-117">Lesen Sie Eigenschaften und Beziehungen des [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="11657-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="11657-118">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="11657-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="11657-119">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="11657-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="11657-120">Ersetzen Sie alle Gruppen für eine Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="11657-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="11657-121">UpdatePriorities Aktion</span><span class="sxs-lookup"><span data-stu-id="11657-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="11657-122">Keines</span><span class="sxs-lookup"><span data-stu-id="11657-122">None</span></span>|<span data-ttu-id="11657-123">Aktualisieren Sie die Richtlinie Prioritäten.</span><span class="sxs-lookup"><span data-stu-id="11657-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="11657-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="11657-124">Properties</span></span>
|<span data-ttu-id="11657-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11657-125">Property</span></span>|<span data-ttu-id="11657-126">Typ</span><span class="sxs-lookup"><span data-stu-id="11657-126">Type</span></span>|<span data-ttu-id="11657-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11657-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11657-128">id</span><span class="sxs-lookup"><span data-stu-id="11657-128">id</span></span>|<span data-ttu-id="11657-129">String</span><span class="sxs-lookup"><span data-stu-id="11657-129">String</span></span>|<span data-ttu-id="11657-130">ID des die Richtlinie Office-Client-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="11657-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="11657-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="11657-131">userPreferencePayload</span></span>|<span data-ttu-id="11657-132">Stream</span><span class="sxs-lookup"><span data-stu-id="11657-132">Stream</span></span>|<span data-ttu-id="11657-133">Vorgaben JSON-Zeichenfolge im Binärformat, können diese Werte vom Benutzer außer Kraft gesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="11657-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="11657-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="11657-134">policyPayload</span></span>|<span data-ttu-id="11657-135">Stream</span><span class="sxs-lookup"><span data-stu-id="11657-135">Stream</span></span>|<span data-ttu-id="11657-136">Richtlinieneinstellungen für JSON-Zeichenfolge im Binärformat, diese Werte können nicht vom Benutzer geändert werden.</span><span class="sxs-lookup"><span data-stu-id="11657-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="11657-137">description</span><span class="sxs-lookup"><span data-stu-id="11657-137">description</span></span>|<span data-ttu-id="11657-138">String</span><span class="sxs-lookup"><span data-stu-id="11657-138">String</span></span>|<span data-ttu-id="11657-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="11657-139">Not yet documented</span></span>|
|<span data-ttu-id="11657-140">displayName</span><span class="sxs-lookup"><span data-stu-id="11657-140">displayName</span></span>|<span data-ttu-id="11657-141">String</span><span class="sxs-lookup"><span data-stu-id="11657-141">String</span></span>|<span data-ttu-id="11657-142">Admin bereitgestellte Beschreibung für den Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="11657-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="11657-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11657-143">lastModifiedDateTime</span></span>|<span data-ttu-id="11657-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="11657-144">DateTime</span></span>|<span data-ttu-id="11657-145">Zuletzt geänderte Datetime-Stempel der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="11657-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="11657-146">Priorität</span><span class="sxs-lookup"><span data-stu-id="11657-146">priority</span></span>|<span data-ttu-id="11657-147">Int32</span><span class="sxs-lookup"><span data-stu-id="11657-147">Int32</span></span>|<span data-ttu-id="11657-148">Prioritätswert sollte eindeutigen Wert für jede Richtlinie unter einem Mandanten sein und für konfliktlösung verwendet werden, niedrigere Werte bedeuten, dass Priorität hoch ist.</span><span class="sxs-lookup"><span data-stu-id="11657-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="11657-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="11657-149">userCheckinSummary</span></span>|[<span data-ttu-id="11657-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="11657-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="11657-151">Benutzer Einchecken Zusammenfassung für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="11657-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="11657-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="11657-152">checkinStatuses</span></span>|<span data-ttu-id="11657-153">[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="11657-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="11657-154">Liste der Office-Client Einchecken Status.</span><span class="sxs-lookup"><span data-stu-id="11657-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11657-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="11657-155">Relationships</span></span>
|<span data-ttu-id="11657-156">Beziehung</span><span class="sxs-lookup"><span data-stu-id="11657-156">Relationship</span></span>|<span data-ttu-id="11657-157">Typ</span><span class="sxs-lookup"><span data-stu-id="11657-157">Type</span></span>|<span data-ttu-id="11657-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11657-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11657-159">assignments</span><span class="sxs-lookup"><span data-stu-id="11657-159">assignments</span></span>|<span data-ttu-id="11657-160">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="11657-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="11657-161">Die Liste der zugewiesenen Gruppe für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="11657-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11657-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="11657-162">JSON Representation</span></span>
<span data-ttu-id="11657-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="11657-163">Here is a JSON representation of the resource.</span></span>
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



