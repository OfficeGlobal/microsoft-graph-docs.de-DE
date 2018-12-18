---
title: Ressourcentyp „managedAppRegistration“
description: ManagedAppEntity ist der Basisentitätstyp für alle anderen Entitätstypen im App-Verwaltungsworkflow.
author: tfitzmac
ms.openlocfilehash: 8a0663ab291dc77568ae91e5a65fab31e809d1a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339858"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="f6a06-103">Ressourcentyp „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="f6a06-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="f6a06-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f6a06-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6a06-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6a06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6a06-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f6a06-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6a06-107">Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="f6a06-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="f6a06-108">Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f6a06-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="f6a06-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="f6a06-109">Methods</span></span>
|<span data-ttu-id="f6a06-110">Methode</span><span class="sxs-lookup"><span data-stu-id="f6a06-110">Method</span></span>|<span data-ttu-id="f6a06-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f6a06-111">Return Type</span></span>|<span data-ttu-id="f6a06-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6a06-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f6a06-113">Auflisten von „managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f6a06-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="f6a06-114">Sammlung von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="f6a06-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="f6a06-115">Listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f6a06-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="f6a06-116">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="f6a06-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="f6a06-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f6a06-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="f6a06-118">Liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="f6a06-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="f6a06-119">Funktion „getUserIdsWithFlaggedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="f6a06-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="f6a06-120">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f6a06-120">String collection</span></span>|<span data-ttu-id="f6a06-121">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f6a06-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f6a06-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f6a06-122">Properties</span></span>
|<span data-ttu-id="f6a06-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6a06-123">Property</span></span>|<span data-ttu-id="f6a06-124">Typ</span><span class="sxs-lookup"><span data-stu-id="f6a06-124">Type</span></span>|<span data-ttu-id="f6a06-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6a06-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6a06-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6a06-126">createdDateTime</span></span>|<span data-ttu-id="f6a06-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6a06-127">DateTimeOffset</span></span>|<span data-ttu-id="f6a06-128">Datum und Uhrzeit der Erstellung</span><span class="sxs-lookup"><span data-stu-id="f6a06-128">Date and time of creation</span></span>|
|<span data-ttu-id="f6a06-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f6a06-129">lastSyncDateTime</span></span>|<span data-ttu-id="f6a06-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6a06-130">DateTimeOffset</span></span>|<span data-ttu-id="f6a06-131">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst</span><span class="sxs-lookup"><span data-stu-id="f6a06-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="f6a06-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="f6a06-132">applicationVersion</span></span>|<span data-ttu-id="f6a06-133">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-133">String</span></span>|<span data-ttu-id="f6a06-134">Version der App</span><span class="sxs-lookup"><span data-stu-id="f6a06-134">App version</span></span>|
|<span data-ttu-id="f6a06-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="f6a06-135">managementSdkVersion</span></span>|<span data-ttu-id="f6a06-136">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-136">String</span></span>|<span data-ttu-id="f6a06-137">Version des App-Verwaltungs-SDK</span><span class="sxs-lookup"><span data-stu-id="f6a06-137">App management SDK version</span></span>|
|<span data-ttu-id="f6a06-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="f6a06-138">platformVersion</span></span>|<span data-ttu-id="f6a06-139">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-139">String</span></span>|<span data-ttu-id="f6a06-140">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="f6a06-140">Operating System version</span></span>|
|<span data-ttu-id="f6a06-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="f6a06-141">deviceType</span></span>|<span data-ttu-id="f6a06-142">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-142">String</span></span>|<span data-ttu-id="f6a06-143">Gerätetyp des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="f6a06-143">Host device type</span></span>|
|<span data-ttu-id="f6a06-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="f6a06-144">deviceTag</span></span>|<span data-ttu-id="f6a06-145">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-145">String</span></span>|<span data-ttu-id="f6a06-146">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="f6a06-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="f6a06-147">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="f6a06-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="f6a06-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="f6a06-148">deviceName</span></span>|<span data-ttu-id="f6a06-149">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-149">String</span></span>|<span data-ttu-id="f6a06-150">Gerätename des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="f6a06-150">Host device name</span></span>|
|<span data-ttu-id="f6a06-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f6a06-151">managedDeviceId</span></span>|<span data-ttu-id="f6a06-152">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-152">String</span></span>|<span data-ttu-id="f6a06-153">Die verwaltete Geräte-ID des Hostgeräts werden soll.</span><span class="sxs-lookup"><span data-stu-id="f6a06-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="f6a06-154">Wert kann leer sein, selbst wenn das Host-Gerät verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="f6a06-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="f6a06-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="f6a06-155">azureADDeviceId</span></span>|<span data-ttu-id="f6a06-156">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-156">String</span></span>|<span data-ttu-id="f6a06-157">Der Azure Active Directory-Gerät Bezeichner des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="f6a06-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="f6a06-158">Wert kann leer sein, auch wenn das Host-Gerät Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="f6a06-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="f6a06-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f6a06-159">deviceModel</span></span>|<span data-ttu-id="f6a06-160">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-160">String</span></span>|<span data-ttu-id="f6a06-161">Das Gerätemodell für die aktuelle app-Registrierung</span><span class="sxs-lookup"><span data-stu-id="f6a06-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="f6a06-162">Einträge deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="f6a06-162">deviceManufacturer</span></span>|<span data-ttu-id="f6a06-163">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-163">String</span></span>|<span data-ttu-id="f6a06-164">Hersteller des Geräts für die aktuelle app-Registrierung</span><span class="sxs-lookup"><span data-stu-id="f6a06-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="f6a06-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="f6a06-165">flaggedReasons</span></span>|<span data-ttu-id="f6a06-166">[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f6a06-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="f6a06-167">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="f6a06-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="f6a06-168">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="f6a06-168">E.g.</span></span> <span data-ttu-id="f6a06-169">Die App wird auf einem gerooteten Gerät ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="f6a06-169">app running on rooted device</span></span>|
|<span data-ttu-id="f6a06-170">userId</span><span class="sxs-lookup"><span data-stu-id="f6a06-170">userId</span></span>|<span data-ttu-id="f6a06-171">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-171">String</span></span>|<span data-ttu-id="f6a06-172">Benutzer-ID, zu der die App-Registrierung gehört</span><span class="sxs-lookup"><span data-stu-id="f6a06-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="f6a06-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="f6a06-173">appIdentifier</span></span>|[<span data-ttu-id="f6a06-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f6a06-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f6a06-175">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="f6a06-175">The app package Identifier</span></span>|
|<span data-ttu-id="f6a06-176">id</span><span class="sxs-lookup"><span data-stu-id="f6a06-176">id</span></span>|<span data-ttu-id="f6a06-177">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-177">String</span></span>|<span data-ttu-id="f6a06-178">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f6a06-178">Key of the entity.</span></span>|
|<span data-ttu-id="f6a06-179">Version</span><span class="sxs-lookup"><span data-stu-id="f6a06-179">version</span></span>|<span data-ttu-id="f6a06-180">String</span><span class="sxs-lookup"><span data-stu-id="f6a06-180">String</span></span>|<span data-ttu-id="f6a06-181">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="f6a06-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6a06-182">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f6a06-182">Relationships</span></span>
|<span data-ttu-id="f6a06-183">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f6a06-183">Relationship</span></span>|<span data-ttu-id="f6a06-184">Typ</span><span class="sxs-lookup"><span data-stu-id="f6a06-184">Type</span></span>|<span data-ttu-id="f6a06-185">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6a06-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6a06-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="f6a06-186">appliedPolicies</span></span>|<span data-ttu-id="f6a06-187">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6a06-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="f6a06-188">Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde</span><span class="sxs-lookup"><span data-stu-id="f6a06-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="f6a06-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="f6a06-189">intendedPolicies</span></span>|<span data-ttu-id="f6a06-190">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6a06-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="f6a06-191">Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat</span><span class="sxs-lookup"><span data-stu-id="f6a06-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="f6a06-192">operations</span><span class="sxs-lookup"><span data-stu-id="f6a06-192">operations</span></span>|<span data-ttu-id="f6a06-193">Sammlung von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="f6a06-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="f6a06-194">Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="f6a06-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6a06-195">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f6a06-195">JSON Representation</span></span>
<span data-ttu-id="f6a06-196">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f6a06-196">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```





