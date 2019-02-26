---
title: Ressourcentyp „managedAppRegistration“
description: Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung. Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63645c7817281f201fd66e39e7fac2c59ff88f5c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151121"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="07dd8-104">Ressourcentyp „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="07dd8-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="07dd8-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07dd8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07dd8-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="07dd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07dd8-107">Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="07dd8-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="07dd8-108">Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="07dd8-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="07dd8-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="07dd8-109">Methods</span></span>
|<span data-ttu-id="07dd8-110">Methode</span><span class="sxs-lookup"><span data-stu-id="07dd8-110">Method</span></span>|<span data-ttu-id="07dd8-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="07dd8-111">Return Type</span></span>|<span data-ttu-id="07dd8-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07dd8-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="07dd8-113">Auflisten von „managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="07dd8-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="07dd8-114">Sammlung von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="07dd8-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="07dd8-115">Listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="07dd8-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="07dd8-116">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="07dd8-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="07dd8-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="07dd8-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="07dd8-118">Liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="07dd8-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="07dd8-119">Funktion „getUserIdsWithFlaggedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="07dd8-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="07dd8-120">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="07dd8-120">String collection</span></span>|<span data-ttu-id="07dd8-121">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="07dd8-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="07dd8-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07dd8-122">Properties</span></span>
|<span data-ttu-id="07dd8-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07dd8-123">Property</span></span>|<span data-ttu-id="07dd8-124">Typ</span><span class="sxs-lookup"><span data-stu-id="07dd8-124">Type</span></span>|<span data-ttu-id="07dd8-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07dd8-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07dd8-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07dd8-126">createdDateTime</span></span>|<span data-ttu-id="07dd8-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07dd8-127">DateTimeOffset</span></span>|<span data-ttu-id="07dd8-128">Datum und Uhrzeit der Erstellung</span><span class="sxs-lookup"><span data-stu-id="07dd8-128">Date and time of creation</span></span>|
|<span data-ttu-id="07dd8-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="07dd8-129">lastSyncDateTime</span></span>|<span data-ttu-id="07dd8-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07dd8-130">DateTimeOffset</span></span>|<span data-ttu-id="07dd8-131">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst</span><span class="sxs-lookup"><span data-stu-id="07dd8-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="07dd8-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="07dd8-132">applicationVersion</span></span>|<span data-ttu-id="07dd8-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07dd8-133">String</span></span>|<span data-ttu-id="07dd8-134">Version der App</span><span class="sxs-lookup"><span data-stu-id="07dd8-134">App version</span></span>|
|<span data-ttu-id="07dd8-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="07dd8-135">managementSdkVersion</span></span>|<span data-ttu-id="07dd8-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07dd8-136">String</span></span>|<span data-ttu-id="07dd8-137">Version des App-Verwaltungs-SDK</span><span class="sxs-lookup"><span data-stu-id="07dd8-137">App management SDK version</span></span>|
|<span data-ttu-id="07dd8-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="07dd8-138">platformVersion</span></span>|<span data-ttu-id="07dd8-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07dd8-139">String</span></span>|<span data-ttu-id="07dd8-140">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="07dd8-140">Operating System version</span></span>|
|<span data-ttu-id="07dd8-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="07dd8-141">deviceType</span></span>|<span data-ttu-id="07dd8-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07dd8-142">String</span></span>|<span data-ttu-id="07dd8-143">Gerätetyp des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="07dd8-143">Host device type</span></span>|
|<span data-ttu-id="07dd8-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="07dd8-144">deviceTag</span></span>|<span data-ttu-id="07dd8-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07dd8-145">String</span></span>|<span data-ttu-id="07dd8-146">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="07dd8-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="07dd8-147">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="07dd8-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="07dd8-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="07dd8-148">deviceName</span></span>|<span data-ttu-id="07dd8-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07dd8-149">String</span></span>|<span data-ttu-id="07dd8-150">Gerätename des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="07dd8-150">Host device name</span></span>|
|<span data-ttu-id="07dd8-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="07dd8-151">managedDeviceId</span></span>|<span data-ttu-id="07dd8-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07dd8-152">String</span></span>|<span data-ttu-id="07dd8-153">Die ID des verwalteten Geräts des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="07dd8-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="07dd8-154">Der Wert kann auch dann leer sein, wenn das Host Gerät verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="07dd8-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="07dd8-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="07dd8-155">azureADDeviceId</span></span>|<span data-ttu-id="07dd8-156">String</span><span class="sxs-lookup"><span data-stu-id="07dd8-156">String</span></span>|<span data-ttu-id="07dd8-157">Die Azure Active Directory-Geräte-ID des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="07dd8-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="07dd8-158">Der Wert kann auch dann leer sein, wenn das Host Gerät Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="07dd8-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="07dd8-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="07dd8-159">deviceModel</span></span>|<span data-ttu-id="07dd8-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07dd8-160">String</span></span>|<span data-ttu-id="07dd8-161">Das Gerätemodell für die aktuelle App-Registrierung</span><span class="sxs-lookup"><span data-stu-id="07dd8-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="07dd8-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="07dd8-162">deviceManufacturer</span></span>|<span data-ttu-id="07dd8-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07dd8-163">String</span></span>|<span data-ttu-id="07dd8-164">Der Gerätehersteller für die aktuelle App-Registrierung</span><span class="sxs-lookup"><span data-stu-id="07dd8-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="07dd8-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="07dd8-165">flaggedReasons</span></span>|<span data-ttu-id="07dd8-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="07dd8-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="07dd8-167">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="07dd8-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="07dd8-168">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="07dd8-168">E.g.</span></span> <span data-ttu-id="07dd8-169">Die App wird auf einem gerooteten Gerät ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="07dd8-169">app running on rooted device</span></span>|
|<span data-ttu-id="07dd8-170">userId</span><span class="sxs-lookup"><span data-stu-id="07dd8-170">userId</span></span>|<span data-ttu-id="07dd8-171">String</span><span class="sxs-lookup"><span data-stu-id="07dd8-171">String</span></span>|<span data-ttu-id="07dd8-172">Benutzer-ID, zu der die App-Registrierung gehört</span><span class="sxs-lookup"><span data-stu-id="07dd8-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="07dd8-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="07dd8-173">appIdentifier</span></span>|[<span data-ttu-id="07dd8-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="07dd8-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="07dd8-175">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="07dd8-175">The app package Identifier</span></span>|
|<span data-ttu-id="07dd8-176">id</span><span class="sxs-lookup"><span data-stu-id="07dd8-176">id</span></span>|<span data-ttu-id="07dd8-177">string</span><span class="sxs-lookup"><span data-stu-id="07dd8-177">String</span></span>|<span data-ttu-id="07dd8-178">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="07dd8-178">Key of the entity.</span></span>|
|<span data-ttu-id="07dd8-179">Version</span><span class="sxs-lookup"><span data-stu-id="07dd8-179">version</span></span>|<span data-ttu-id="07dd8-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07dd8-180">String</span></span>|<span data-ttu-id="07dd8-181">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="07dd8-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07dd8-182">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="07dd8-182">Relationships</span></span>
|<span data-ttu-id="07dd8-183">Beziehung</span><span class="sxs-lookup"><span data-stu-id="07dd8-183">Relationship</span></span>|<span data-ttu-id="07dd8-184">Typ</span><span class="sxs-lookup"><span data-stu-id="07dd8-184">Type</span></span>|<span data-ttu-id="07dd8-185">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07dd8-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07dd8-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="07dd8-186">appliedPolicies</span></span>|<span data-ttu-id="07dd8-187">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="07dd8-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="07dd8-188">Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde</span><span class="sxs-lookup"><span data-stu-id="07dd8-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="07dd8-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="07dd8-189">intendedPolicies</span></span>|<span data-ttu-id="07dd8-190">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="07dd8-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="07dd8-191">Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat</span><span class="sxs-lookup"><span data-stu-id="07dd8-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="07dd8-192">operations</span><span class="sxs-lookup"><span data-stu-id="07dd8-192">operations</span></span>|<span data-ttu-id="07dd8-193">Sammlung von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="07dd8-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="07dd8-194">Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="07dd8-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07dd8-195">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07dd8-195">JSON Representation</span></span>
<span data-ttu-id="07dd8-196">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07dd8-196">Here is a JSON representation of the resource.</span></span>
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




