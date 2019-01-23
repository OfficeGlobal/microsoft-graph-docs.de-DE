---
title: Ressourcentyp „managedAppRegistration“
description: Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung. Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a343dba3df1274693449b8f7cbefd83b131138c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421438"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="9add4-104">Ressourcentyp „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="9add4-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="9add4-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9add4-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9add4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9add4-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9add4-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9add4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9add4-108">Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="9add4-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="9add4-109">Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9add4-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="9add4-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="9add4-110">Methods</span></span>
|<span data-ttu-id="9add4-111">Methode</span><span class="sxs-lookup"><span data-stu-id="9add4-111">Method</span></span>|<span data-ttu-id="9add4-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9add4-112">Return Type</span></span>|<span data-ttu-id="9add4-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9add4-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9add4-114">Auflisten von „managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9add4-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="9add4-115">Sammlung von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="9add4-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="9add4-116">Listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="9add4-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="9add4-117">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="9add4-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="9add4-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9add4-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="9add4-119">Liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9add4-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="9add4-120">Funktion „getUserIdsWithFlaggedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="9add4-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="9add4-121">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9add4-121">String collection</span></span>|<span data-ttu-id="9add4-122">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9add4-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9add4-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9add4-123">Properties</span></span>
|<span data-ttu-id="9add4-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9add4-124">Property</span></span>|<span data-ttu-id="9add4-125">Typ</span><span class="sxs-lookup"><span data-stu-id="9add4-125">Type</span></span>|<span data-ttu-id="9add4-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9add4-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9add4-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9add4-127">createdDateTime</span></span>|<span data-ttu-id="9add4-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9add4-128">DateTimeOffset</span></span>|<span data-ttu-id="9add4-129">Datum und Uhrzeit der Erstellung</span><span class="sxs-lookup"><span data-stu-id="9add4-129">Date and time of creation</span></span>|
|<span data-ttu-id="9add4-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9add4-130">lastSyncDateTime</span></span>|<span data-ttu-id="9add4-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9add4-131">DateTimeOffset</span></span>|<span data-ttu-id="9add4-132">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst</span><span class="sxs-lookup"><span data-stu-id="9add4-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="9add4-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="9add4-133">applicationVersion</span></span>|<span data-ttu-id="9add4-134">String</span><span class="sxs-lookup"><span data-stu-id="9add4-134">String</span></span>|<span data-ttu-id="9add4-135">Version der App</span><span class="sxs-lookup"><span data-stu-id="9add4-135">App version</span></span>|
|<span data-ttu-id="9add4-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="9add4-136">managementSdkVersion</span></span>|<span data-ttu-id="9add4-137">String</span><span class="sxs-lookup"><span data-stu-id="9add4-137">String</span></span>|<span data-ttu-id="9add4-138">Version des App-Verwaltungs-SDK</span><span class="sxs-lookup"><span data-stu-id="9add4-138">App management SDK version</span></span>|
|<span data-ttu-id="9add4-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="9add4-139">platformVersion</span></span>|<span data-ttu-id="9add4-140">String</span><span class="sxs-lookup"><span data-stu-id="9add4-140">String</span></span>|<span data-ttu-id="9add4-141">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="9add4-141">Operating System version</span></span>|
|<span data-ttu-id="9add4-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="9add4-142">deviceType</span></span>|<span data-ttu-id="9add4-143">String</span><span class="sxs-lookup"><span data-stu-id="9add4-143">String</span></span>|<span data-ttu-id="9add4-144">Gerätetyp des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="9add4-144">Host device type</span></span>|
|<span data-ttu-id="9add4-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="9add4-145">deviceTag</span></span>|<span data-ttu-id="9add4-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9add4-146">String</span></span>|<span data-ttu-id="9add4-147">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="9add4-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="9add4-148">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="9add4-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="9add4-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="9add4-149">deviceName</span></span>|<span data-ttu-id="9add4-150">String</span><span class="sxs-lookup"><span data-stu-id="9add4-150">String</span></span>|<span data-ttu-id="9add4-151">Gerätename des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="9add4-151">Host device name</span></span>|
|<span data-ttu-id="9add4-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="9add4-152">managedDeviceId</span></span>|<span data-ttu-id="9add4-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9add4-153">String</span></span>|<span data-ttu-id="9add4-154">Die verwaltete Geräte-ID des Hostgeräts werden soll.</span><span class="sxs-lookup"><span data-stu-id="9add4-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="9add4-155">Wert kann leer sein, selbst wenn das Host-Gerät verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="9add4-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="9add4-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="9add4-156">azureADDeviceId</span></span>|<span data-ttu-id="9add4-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9add4-157">String</span></span>|<span data-ttu-id="9add4-158">Der Azure Active Directory-Gerät Bezeichner des Hostgeräts.</span><span class="sxs-lookup"><span data-stu-id="9add4-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="9add4-159">Wert kann leer sein, auch wenn das Host-Gerät Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="9add4-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="9add4-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9add4-160">deviceModel</span></span>|<span data-ttu-id="9add4-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9add4-161">String</span></span>|<span data-ttu-id="9add4-162">Das Gerätemodell für die aktuelle app-Registrierung</span><span class="sxs-lookup"><span data-stu-id="9add4-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="9add4-163">Einträge deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="9add4-163">deviceManufacturer</span></span>|<span data-ttu-id="9add4-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9add4-164">String</span></span>|<span data-ttu-id="9add4-165">Hersteller des Geräts für die aktuelle app-Registrierung</span><span class="sxs-lookup"><span data-stu-id="9add4-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="9add4-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="9add4-166">flaggedReasons</span></span>|<span data-ttu-id="9add4-167">[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9add4-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="9add4-168">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="9add4-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="9add4-169">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="9add4-169">E.g.</span></span> <span data-ttu-id="9add4-170">Die App wird auf einem gerooteten Gerät ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9add4-170">app running on rooted device</span></span>|
|<span data-ttu-id="9add4-171">userId</span><span class="sxs-lookup"><span data-stu-id="9add4-171">userId</span></span>|<span data-ttu-id="9add4-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9add4-172">String</span></span>|<span data-ttu-id="9add4-173">Benutzer-ID, zu der die App-Registrierung gehört</span><span class="sxs-lookup"><span data-stu-id="9add4-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="9add4-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="9add4-174">appIdentifier</span></span>|[<span data-ttu-id="9add4-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9add4-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9add4-176">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="9add4-176">The app package Identifier</span></span>|
|<span data-ttu-id="9add4-177">id</span><span class="sxs-lookup"><span data-stu-id="9add4-177">id</span></span>|<span data-ttu-id="9add4-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9add4-178">String</span></span>|<span data-ttu-id="9add4-179">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9add4-179">Key of the entity.</span></span>|
|<span data-ttu-id="9add4-180">Version</span><span class="sxs-lookup"><span data-stu-id="9add4-180">version</span></span>|<span data-ttu-id="9add4-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9add4-181">String</span></span>|<span data-ttu-id="9add4-182">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="9add4-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9add4-183">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9add4-183">Relationships</span></span>
|<span data-ttu-id="9add4-184">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9add4-184">Relationship</span></span>|<span data-ttu-id="9add4-185">Typ</span><span class="sxs-lookup"><span data-stu-id="9add4-185">Type</span></span>|<span data-ttu-id="9add4-186">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9add4-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9add4-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="9add4-187">appliedPolicies</span></span>|<span data-ttu-id="9add4-188">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9add4-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="9add4-189">Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde</span><span class="sxs-lookup"><span data-stu-id="9add4-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="9add4-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="9add4-190">intendedPolicies</span></span>|<span data-ttu-id="9add4-191">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9add4-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="9add4-192">Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat</span><span class="sxs-lookup"><span data-stu-id="9add4-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="9add4-193">operations</span><span class="sxs-lookup"><span data-stu-id="9add4-193">operations</span></span>|<span data-ttu-id="9add4-194">Sammlung von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9add4-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="9add4-195">Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="9add4-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9add4-196">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9add4-196">JSON Representation</span></span>
<span data-ttu-id="9add4-197">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9add4-197">Here is a JSON representation of the resource.</span></span>
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




