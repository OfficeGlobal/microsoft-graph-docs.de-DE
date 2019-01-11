---
title: Ressourcentyp „managedAppRegistration“
description: ManagedAppEntity ist der Basisentitätstyp für alle anderen Entitätstypen im App-Verwaltungsworkflow.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 959bd294ab1752617cea6a6ea5bbe8f0a3802f0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869720"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="72b46-103">Ressourcentyp „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="72b46-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="72b46-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="72b46-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72b46-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="72b46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72b46-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="72b46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72b46-107">Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="72b46-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="72b46-108">Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="72b46-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="72b46-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="72b46-109">Methods</span></span>
|<span data-ttu-id="72b46-110">Methode</span><span class="sxs-lookup"><span data-stu-id="72b46-110">Method</span></span>|<span data-ttu-id="72b46-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="72b46-111">Return Type</span></span>|<span data-ttu-id="72b46-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72b46-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="72b46-113">Auflisten von „managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="72b46-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="72b46-114">Sammlung von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="72b46-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="72b46-115">Listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="72b46-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="72b46-116">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="72b46-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="72b46-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="72b46-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="72b46-118">Liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="72b46-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="72b46-119">Funktion „getUserIdsWithFlaggedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="72b46-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="72b46-120">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="72b46-120">String collection</span></span>|<span data-ttu-id="72b46-121">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="72b46-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="72b46-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="72b46-122">Properties</span></span>
|<span data-ttu-id="72b46-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="72b46-123">Property</span></span>|<span data-ttu-id="72b46-124">Typ</span><span class="sxs-lookup"><span data-stu-id="72b46-124">Type</span></span>|<span data-ttu-id="72b46-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72b46-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72b46-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72b46-126">createdDateTime</span></span>|<span data-ttu-id="72b46-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b46-127">DateTimeOffset</span></span>|<span data-ttu-id="72b46-128">Datum und Uhrzeit der Erstellung</span><span class="sxs-lookup"><span data-stu-id="72b46-128">Date and time of creation</span></span>|
|<span data-ttu-id="72b46-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="72b46-129">lastSyncDateTime</span></span>|<span data-ttu-id="72b46-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b46-130">DateTimeOffset</span></span>|<span data-ttu-id="72b46-131">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst</span><span class="sxs-lookup"><span data-stu-id="72b46-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="72b46-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="72b46-132">applicationVersion</span></span>|<span data-ttu-id="72b46-133">String</span><span class="sxs-lookup"><span data-stu-id="72b46-133">String</span></span>|<span data-ttu-id="72b46-134">Version der App</span><span class="sxs-lookup"><span data-stu-id="72b46-134">App version</span></span>|
|<span data-ttu-id="72b46-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="72b46-135">managementSdkVersion</span></span>|<span data-ttu-id="72b46-136">String</span><span class="sxs-lookup"><span data-stu-id="72b46-136">String</span></span>|<span data-ttu-id="72b46-137">Version des App-Verwaltungs-SDK</span><span class="sxs-lookup"><span data-stu-id="72b46-137">App management SDK version</span></span>|
|<span data-ttu-id="72b46-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="72b46-138">platformVersion</span></span>|<span data-ttu-id="72b46-139">String</span><span class="sxs-lookup"><span data-stu-id="72b46-139">String</span></span>|<span data-ttu-id="72b46-140">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="72b46-140">Operating System version</span></span>|
|<span data-ttu-id="72b46-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="72b46-141">deviceType</span></span>|<span data-ttu-id="72b46-142">String</span><span class="sxs-lookup"><span data-stu-id="72b46-142">String</span></span>|<span data-ttu-id="72b46-143">Gerätetyp des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="72b46-143">Host device type</span></span>|
|<span data-ttu-id="72b46-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="72b46-144">deviceTag</span></span>|<span data-ttu-id="72b46-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72b46-145">String</span></span>|<span data-ttu-id="72b46-146">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="72b46-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="72b46-147">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="72b46-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="72b46-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="72b46-148">deviceName</span></span>|<span data-ttu-id="72b46-149">String</span><span class="sxs-lookup"><span data-stu-id="72b46-149">String</span></span>|<span data-ttu-id="72b46-150">Gerätename des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="72b46-150">Host device name</span></span>|
|<span data-ttu-id="72b46-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="72b46-151">managedDeviceId</span></span>|<span data-ttu-id="72b46-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72b46-152">String</span></span>|<span data-ttu-id="72b46-153">Die verwaltete Geräte-ID des Hostgeräts werden soll.</span><span class="sxs-lookup"><span data-stu-id="72b46-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="72b46-154">Wert kann leer sein, selbst wenn das Host-Gerät verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="72b46-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="72b46-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="72b46-155">azureADDeviceId</span></span>|<span data-ttu-id="72b46-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72b46-156">String</span></span>|<span data-ttu-id="72b46-157">Der Azure Active Directory-Gerät Bezeichner des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="72b46-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="72b46-158">Wert kann leer sein, auch wenn das Host-Gerät Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="72b46-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="72b46-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="72b46-159">deviceModel</span></span>|<span data-ttu-id="72b46-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72b46-160">String</span></span>|<span data-ttu-id="72b46-161">Das Gerätemodell für die aktuelle app-Registrierung</span><span class="sxs-lookup"><span data-stu-id="72b46-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="72b46-162">Einträge deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="72b46-162">deviceManufacturer</span></span>|<span data-ttu-id="72b46-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72b46-163">String</span></span>|<span data-ttu-id="72b46-164">Hersteller des Geräts für die aktuelle app-Registrierung</span><span class="sxs-lookup"><span data-stu-id="72b46-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="72b46-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="72b46-165">flaggedReasons</span></span>|<span data-ttu-id="72b46-166">[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="72b46-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="72b46-167">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="72b46-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="72b46-168">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="72b46-168">E.g.</span></span> <span data-ttu-id="72b46-169">Die App wird auf einem gerooteten Gerät ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="72b46-169">app running on rooted device</span></span>|
|<span data-ttu-id="72b46-170">userId</span><span class="sxs-lookup"><span data-stu-id="72b46-170">userId</span></span>|<span data-ttu-id="72b46-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72b46-171">String</span></span>|<span data-ttu-id="72b46-172">Benutzer-ID, zu der die App-Registrierung gehört</span><span class="sxs-lookup"><span data-stu-id="72b46-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="72b46-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="72b46-173">appIdentifier</span></span>|[<span data-ttu-id="72b46-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="72b46-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="72b46-175">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="72b46-175">The app package Identifier</span></span>|
|<span data-ttu-id="72b46-176">id</span><span class="sxs-lookup"><span data-stu-id="72b46-176">id</span></span>|<span data-ttu-id="72b46-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72b46-177">String</span></span>|<span data-ttu-id="72b46-178">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="72b46-178">Key of the entity.</span></span>|
|<span data-ttu-id="72b46-179">Version</span><span class="sxs-lookup"><span data-stu-id="72b46-179">version</span></span>|<span data-ttu-id="72b46-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72b46-180">String</span></span>|<span data-ttu-id="72b46-181">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="72b46-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72b46-182">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="72b46-182">Relationships</span></span>
|<span data-ttu-id="72b46-183">Beziehung</span><span class="sxs-lookup"><span data-stu-id="72b46-183">Relationship</span></span>|<span data-ttu-id="72b46-184">Typ</span><span class="sxs-lookup"><span data-stu-id="72b46-184">Type</span></span>|<span data-ttu-id="72b46-185">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72b46-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72b46-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="72b46-186">appliedPolicies</span></span>|<span data-ttu-id="72b46-187">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="72b46-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="72b46-188">Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde</span><span class="sxs-lookup"><span data-stu-id="72b46-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="72b46-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="72b46-189">intendedPolicies</span></span>|<span data-ttu-id="72b46-190">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="72b46-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="72b46-191">Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat</span><span class="sxs-lookup"><span data-stu-id="72b46-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="72b46-192">operations</span><span class="sxs-lookup"><span data-stu-id="72b46-192">operations</span></span>|<span data-ttu-id="72b46-193">Sammlung von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="72b46-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="72b46-194">Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="72b46-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72b46-195">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="72b46-195">JSON Representation</span></span>
<span data-ttu-id="72b46-196">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="72b46-196">Here is a JSON representation of the resource.</span></span>
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





