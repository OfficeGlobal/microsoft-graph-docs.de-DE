---
title: Ressourcentyp „managedAppRegistration“
description: ManagedAppEntity ist der Basisentitätstyp für alle anderen Entitätstypen im App-Verwaltungsworkflow.
author: tfitzmac
ms.openlocfilehash: 218a36a283febe646afcc6f9c9bcbd0ed5abf46a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347789"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="16d40-103">Ressourcentyp „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="16d40-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="16d40-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="16d40-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16d40-105">Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="16d40-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="16d40-106">Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="16d40-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="16d40-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="16d40-107">Methods</span></span>
|<span data-ttu-id="16d40-108">Methode</span><span class="sxs-lookup"><span data-stu-id="16d40-108">Method</span></span>|<span data-ttu-id="16d40-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="16d40-109">Return Type</span></span>|<span data-ttu-id="16d40-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16d40-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="16d40-111">Auflisten von „managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="16d40-111">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="16d40-112">Sammlung von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="16d40-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="16d40-113">Listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="16d40-113">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="16d40-114">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="16d40-114">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="16d40-115">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="16d40-115">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="16d40-116">Liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="16d40-116">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="16d40-117">Funktion „getUserIdsWithFlaggedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="16d40-117">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="16d40-118">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="16d40-118">String collection</span></span>|<span data-ttu-id="16d40-119">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="16d40-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="16d40-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16d40-120">Properties</span></span>
|<span data-ttu-id="16d40-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16d40-121">Property</span></span>|<span data-ttu-id="16d40-122">Typ</span><span class="sxs-lookup"><span data-stu-id="16d40-122">Type</span></span>|<span data-ttu-id="16d40-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16d40-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16d40-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16d40-124">createdDateTime</span></span>|<span data-ttu-id="16d40-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16d40-125">DateTimeOffset</span></span>|<span data-ttu-id="16d40-126">Datum und Uhrzeit der Erstellung</span><span class="sxs-lookup"><span data-stu-id="16d40-126">Date and time of creation</span></span>|
|<span data-ttu-id="16d40-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="16d40-127">lastSyncDateTime</span></span>|<span data-ttu-id="16d40-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16d40-128">DateTimeOffset</span></span>|<span data-ttu-id="16d40-129">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst</span><span class="sxs-lookup"><span data-stu-id="16d40-129">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="16d40-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="16d40-130">applicationVersion</span></span>|<span data-ttu-id="16d40-131">String</span><span class="sxs-lookup"><span data-stu-id="16d40-131">String</span></span>|<span data-ttu-id="16d40-132">Version der App</span><span class="sxs-lookup"><span data-stu-id="16d40-132">App version</span></span>|
|<span data-ttu-id="16d40-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="16d40-133">managementSdkVersion</span></span>|<span data-ttu-id="16d40-134">String</span><span class="sxs-lookup"><span data-stu-id="16d40-134">String</span></span>|<span data-ttu-id="16d40-135">Version des App-Verwaltungs-SDK</span><span class="sxs-lookup"><span data-stu-id="16d40-135">App management SDK version</span></span>|
|<span data-ttu-id="16d40-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="16d40-136">platformVersion</span></span>|<span data-ttu-id="16d40-137">String</span><span class="sxs-lookup"><span data-stu-id="16d40-137">String</span></span>|<span data-ttu-id="16d40-138">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="16d40-138">Operating System version</span></span>|
|<span data-ttu-id="16d40-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="16d40-139">deviceType</span></span>|<span data-ttu-id="16d40-140">String</span><span class="sxs-lookup"><span data-stu-id="16d40-140">String</span></span>|<span data-ttu-id="16d40-141">Gerätetyp des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="16d40-141">Host device type</span></span>|
|<span data-ttu-id="16d40-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="16d40-142">deviceTag</span></span>|<span data-ttu-id="16d40-143">String</span><span class="sxs-lookup"><span data-stu-id="16d40-143">String</span></span>|<span data-ttu-id="16d40-144">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="16d40-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="16d40-145">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="16d40-145">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="16d40-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="16d40-146">deviceName</span></span>|<span data-ttu-id="16d40-147">String</span><span class="sxs-lookup"><span data-stu-id="16d40-147">String</span></span>|<span data-ttu-id="16d40-148">Gerätename des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="16d40-148">Host device name</span></span>|
|<span data-ttu-id="16d40-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="16d40-149">flaggedReasons</span></span>|<span data-ttu-id="16d40-150">[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="16d40-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="16d40-151">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="16d40-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="16d40-152">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="16d40-152">E.g.</span></span> <span data-ttu-id="16d40-153">Die App wird auf einem gerooteten Gerät ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="16d40-153">app running on rooted device</span></span>|
|<span data-ttu-id="16d40-154">userId</span><span class="sxs-lookup"><span data-stu-id="16d40-154">userId</span></span>|<span data-ttu-id="16d40-155">String</span><span class="sxs-lookup"><span data-stu-id="16d40-155">String</span></span>|<span data-ttu-id="16d40-156">Benutzer-ID, zu der die App-Registrierung gehört</span><span class="sxs-lookup"><span data-stu-id="16d40-156">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="16d40-157">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="16d40-157">appIdentifier</span></span>|[<span data-ttu-id="16d40-158">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="16d40-158">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="16d40-159">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="16d40-159">The app package Identifier</span></span>|
|<span data-ttu-id="16d40-160">id</span><span class="sxs-lookup"><span data-stu-id="16d40-160">id</span></span>|<span data-ttu-id="16d40-161">String</span><span class="sxs-lookup"><span data-stu-id="16d40-161">String</span></span>|<span data-ttu-id="16d40-162">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="16d40-162">Key of the entity.</span></span>|
|<span data-ttu-id="16d40-163">Version</span><span class="sxs-lookup"><span data-stu-id="16d40-163">version</span></span>|<span data-ttu-id="16d40-164">String</span><span class="sxs-lookup"><span data-stu-id="16d40-164">String</span></span>|<span data-ttu-id="16d40-165">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="16d40-165">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16d40-166">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="16d40-166">Relationships</span></span>
|<span data-ttu-id="16d40-167">Beziehung</span><span class="sxs-lookup"><span data-stu-id="16d40-167">Relationship</span></span>|<span data-ttu-id="16d40-168">Typ</span><span class="sxs-lookup"><span data-stu-id="16d40-168">Type</span></span>|<span data-ttu-id="16d40-169">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16d40-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16d40-170">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="16d40-170">appliedPolicies</span></span>|<span data-ttu-id="16d40-171">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16d40-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="16d40-172">Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde</span><span class="sxs-lookup"><span data-stu-id="16d40-172">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="16d40-173">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="16d40-173">intendedPolicies</span></span>|<span data-ttu-id="16d40-174">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16d40-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="16d40-175">Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat</span><span class="sxs-lookup"><span data-stu-id="16d40-175">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="16d40-176">operations</span><span class="sxs-lookup"><span data-stu-id="16d40-176">operations</span></span>|<span data-ttu-id="16d40-177">Sammlung von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="16d40-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="16d40-178">Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="16d40-178">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16d40-179">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16d40-179">JSON Representation</span></span>
<span data-ttu-id="16d40-180">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="16d40-180">Here is a JSON representation of the resource.</span></span>
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


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
