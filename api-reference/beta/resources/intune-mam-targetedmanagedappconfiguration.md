---
title: targetedManagedAppConfiguration-Ressourcentyp
description: Konfiguration für das Übermitteln eines Satzes benutzerdefinierter Einstellungen an alle Benutzer in der Zielsicherheitsgruppe.
ms.openlocfilehash: 9ddd84e07b76e6e9a8915cde14f4194228fdfb3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062222"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="3bef9-103">targetedManagedAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3bef9-103">targetedManagedAppConfiguration resource type</span></span>

> <span data-ttu-id="3bef9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3bef9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bef9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3bef9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3bef9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3bef9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3bef9-107">Konfiguration für das Übermitteln eines Satzes benutzerdefinierter Einstellungen an alle Benutzer in der Zielsicherheitsgruppe.</span><span class="sxs-lookup"><span data-stu-id="3bef9-107">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>

<span data-ttu-id="3bef9-108">Erbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bef9-108">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3bef9-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="3bef9-109">Methods</span></span>
|<span data-ttu-id="3bef9-110">Methode</span><span class="sxs-lookup"><span data-stu-id="3bef9-110">Method</span></span>|<span data-ttu-id="3bef9-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3bef9-111">Return Type</span></span>|<span data-ttu-id="3bef9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bef9-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3bef9-113">targetedManagedAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="3bef9-113">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="3bef9-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3bef9-114">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="3bef9-115">Auflisten von Eigenschaften und Beziehungen der [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="3bef9-115">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3bef9-116">TargetedManagedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="3bef9-116">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="3bef9-117">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bef9-117">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="3bef9-118">Lesen von Eigenschaften und Beziehungen des [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3bef9-118">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3bef9-119">TargetedManagedAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="3bef9-119">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="3bef9-120">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bef9-120">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="3bef9-121">Erstellen eines neuen [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3bef9-121">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3bef9-122">TargetedManagedAppConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="3bef9-122">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="3bef9-123">Keine</span><span class="sxs-lookup"><span data-stu-id="3bef9-123">None</span></span>|<span data-ttu-id="3bef9-124">Löscht ein [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="3bef9-124">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="3bef9-125">TargetedManagedAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3bef9-125">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="3bef9-126">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bef9-126">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="3bef9-127">Aktualisieren der Eigenschaften eines [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)- Objekts.</span><span class="sxs-lookup"><span data-stu-id="3bef9-127">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3bef9-128">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="3bef9-128">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="3bef9-129">Keine</span><span class="sxs-lookup"><span data-stu-id="3bef9-129">None</span></span>|<span data-ttu-id="3bef9-130">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3bef9-130">Not yet documented</span></span>|
|[<span data-ttu-id="3bef9-131">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="3bef9-131">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="3bef9-132">Keine</span><span class="sxs-lookup"><span data-stu-id="3bef9-132">None</span></span>|<span data-ttu-id="3bef9-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3bef9-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3bef9-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3bef9-134">Properties</span></span>
|<span data-ttu-id="3bef9-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3bef9-135">Property</span></span>|<span data-ttu-id="3bef9-136">Typ</span><span class="sxs-lookup"><span data-stu-id="3bef9-136">Type</span></span>|<span data-ttu-id="3bef9-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bef9-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bef9-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3bef9-138">displayName</span></span>|<span data-ttu-id="3bef9-139">String</span><span class="sxs-lookup"><span data-stu-id="3bef9-139">String</span></span>|<span data-ttu-id="3bef9-140">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3bef9-140">Policy display name.</span></span> <span data-ttu-id="3bef9-141">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3bef9-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3bef9-142">description</span><span class="sxs-lookup"><span data-stu-id="3bef9-142">description</span></span>|<span data-ttu-id="3bef9-143">String</span><span class="sxs-lookup"><span data-stu-id="3bef9-143">String</span></span>|<span data-ttu-id="3bef9-144">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3bef9-144">The policy's description.</span></span> <span data-ttu-id="3bef9-145">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3bef9-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3bef9-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bef9-146">createdDateTime</span></span>|<span data-ttu-id="3bef9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bef9-147">DateTimeOffset</span></span>|<span data-ttu-id="3bef9-148">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3bef9-148">The date and time the policy was created.</span></span> <span data-ttu-id="3bef9-149">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3bef9-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3bef9-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bef9-150">lastModifiedDateTime</span></span>|<span data-ttu-id="3bef9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bef9-151">DateTimeOffset</span></span>|<span data-ttu-id="3bef9-152">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="3bef9-152">Last time the policy was modified.</span></span> <span data-ttu-id="3bef9-153">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3bef9-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3bef9-154">id</span><span class="sxs-lookup"><span data-stu-id="3bef9-154">id</span></span>|<span data-ttu-id="3bef9-155">String</span><span class="sxs-lookup"><span data-stu-id="3bef9-155">String</span></span>|<span data-ttu-id="3bef9-156">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3bef9-156">Key of the entity.</span></span> <span data-ttu-id="3bef9-157">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3bef9-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3bef9-158">Version</span><span class="sxs-lookup"><span data-stu-id="3bef9-158">version</span></span>|<span data-ttu-id="3bef9-159">String</span><span class="sxs-lookup"><span data-stu-id="3bef9-159">String</span></span>|<span data-ttu-id="3bef9-160">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="3bef9-160">Version of the entity.</span></span> <span data-ttu-id="3bef9-161">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3bef9-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3bef9-162">customSettings</span><span class="sxs-lookup"><span data-stu-id="3bef9-162">customSettings</span></span>|<span data-ttu-id="3bef9-163">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3bef9-163">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3bef9-164">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bef9-164">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="3bef9-165">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="3bef9-165">deployedAppCount</span></span>|<span data-ttu-id="3bef9-166">Int32</span><span class="sxs-lookup"><span data-stu-id="3bef9-166">Int32</span></span>|<span data-ttu-id="3bef9-167">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3bef9-167">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="3bef9-168">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3bef9-168">isAssigned</span></span>|<span data-ttu-id="3bef9-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3bef9-169">Boolean</span></span>|<span data-ttu-id="3bef9-170">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3bef9-170">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bef9-171">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3bef9-171">Relationships</span></span>
|<span data-ttu-id="3bef9-172">Beziehung</span><span class="sxs-lookup"><span data-stu-id="3bef9-172">Relationship</span></span>|<span data-ttu-id="3bef9-173">Typ</span><span class="sxs-lookup"><span data-stu-id="3bef9-173">Type</span></span>|<span data-ttu-id="3bef9-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bef9-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bef9-175">Apps</span><span class="sxs-lookup"><span data-stu-id="3bef9-175">apps</span></span>|<span data-ttu-id="3bef9-176">Sammlung von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bef9-176">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="3bef9-177">Liste der Apps, für die die Richtlinie bereitgestellt wurde</span><span class="sxs-lookup"><span data-stu-id="3bef9-177">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="3bef9-178">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="3bef9-178">deploymentSummary</span></span>|[<span data-ttu-id="3bef9-179">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="3bef9-179">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="3bef9-180">Navigationseigenschaft zu einer Bereitstellungsübersicht für die Konfiguration</span><span class="sxs-lookup"><span data-stu-id="3bef9-180">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="3bef9-181">assignments</span><span class="sxs-lookup"><span data-stu-id="3bef9-181">assignments</span></span>|<span data-ttu-id="3bef9-182">Sammlung von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3bef9-182">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="3bef9-183">Navigationseigenschaft zu einer Liste von Einschlussgruppen und Ausschlussgruppen, für die die Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3bef9-183">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3bef9-184">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3bef9-184">JSON Representation</span></span>
<span data-ttu-id="3bef9-185">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3bef9-185">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```




