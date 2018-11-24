# <a name="managedappregistration-resource-type"></a><span data-ttu-id="91813-101">Ressourcentyp „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="91813-101">managedAppRegistration resource type</span></span>

> <span data-ttu-id="91813-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="91813-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91813-103">Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="91813-103">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="91813-104">Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="91813-104">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="91813-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="91813-105">Methods</span></span>
|<span data-ttu-id="91813-106">Methode</span><span class="sxs-lookup"><span data-stu-id="91813-106">Method</span></span>|<span data-ttu-id="91813-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="91813-107">Return Type</span></span>|<span data-ttu-id="91813-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91813-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91813-109">Auflisten von „managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="91813-109">List managedAppRegistrations</span></span>](../api/intune_mam_managedappregistration_list.md)|<span data-ttu-id="91813-110">Sammlung von Objekten des Typs [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="91813-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="91813-111">Listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune_mam_managedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="91813-111">List properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="91813-112">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="91813-112">Get managedAppRegistration</span></span>](../api/intune_mam_managedappregistration_get.md)|[<span data-ttu-id="91813-113">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="91813-113">managedAppRegistration</span></span>](../resources/intune_mam_managedappregistration.md)|<span data-ttu-id="91813-114">Liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="91813-114">Read properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="91813-115">Funktion „getUserIdsWithFlaggedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="91813-115">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|<span data-ttu-id="91813-116">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="91813-116">String collection</span></span>|<span data-ttu-id="91813-117">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="91813-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="91813-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91813-118">Properties</span></span>
|<span data-ttu-id="91813-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91813-119">Property</span></span>|<span data-ttu-id="91813-120">Typ</span><span class="sxs-lookup"><span data-stu-id="91813-120">Type</span></span>|<span data-ttu-id="91813-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91813-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91813-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91813-122">createdDateTime</span></span>|<span data-ttu-id="91813-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91813-123">DateTimeOffset</span></span>|<span data-ttu-id="91813-124">Datum und Uhrzeit der Erstellung</span><span class="sxs-lookup"><span data-stu-id="91813-124">Date and time of creation</span></span>|
|<span data-ttu-id="91813-125">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="91813-125">lastSyncDateTime</span></span>|<span data-ttu-id="91813-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91813-126">DateTimeOffset</span></span>|<span data-ttu-id="91813-127">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst</span><span class="sxs-lookup"><span data-stu-id="91813-127">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="91813-128">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="91813-128">applicationVersion</span></span>|<span data-ttu-id="91813-129">String</span><span class="sxs-lookup"><span data-stu-id="91813-129">String</span></span>|<span data-ttu-id="91813-130">Version der App</span><span class="sxs-lookup"><span data-stu-id="91813-130">App version</span></span>|
|<span data-ttu-id="91813-131">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="91813-131">managementSdkVersion</span></span>|<span data-ttu-id="91813-132">String</span><span class="sxs-lookup"><span data-stu-id="91813-132">String</span></span>|<span data-ttu-id="91813-133">Version des App-Verwaltungs-SDK</span><span class="sxs-lookup"><span data-stu-id="91813-133">App management SDK version</span></span>|
|<span data-ttu-id="91813-134">platformVersion</span><span class="sxs-lookup"><span data-stu-id="91813-134">platformVersion</span></span>|<span data-ttu-id="91813-135">String</span><span class="sxs-lookup"><span data-stu-id="91813-135">String</span></span>|<span data-ttu-id="91813-136">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="91813-136">Operating System version</span></span>|
|<span data-ttu-id="91813-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="91813-137">deviceType</span></span>|<span data-ttu-id="91813-138">String</span><span class="sxs-lookup"><span data-stu-id="91813-138">String</span></span>|<span data-ttu-id="91813-139">Gerätetyp des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="91813-139">Host device type</span></span>|
|<span data-ttu-id="91813-140">deviceTag</span><span class="sxs-lookup"><span data-stu-id="91813-140">deviceTag</span></span>|<span data-ttu-id="91813-141">String</span><span class="sxs-lookup"><span data-stu-id="91813-141">String</span></span>|<span data-ttu-id="91813-142">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="91813-142">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="91813-143">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="91813-143">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="91813-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="91813-144">deviceName</span></span>|<span data-ttu-id="91813-145">String</span><span class="sxs-lookup"><span data-stu-id="91813-145">String</span></span>|<span data-ttu-id="91813-146">Gerätename des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="91813-146">Host device name</span></span>|
|<span data-ttu-id="91813-147">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="91813-147">flaggedReasons</span></span>|<span data-ttu-id="91813-148">[ManagedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="91813-148">[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="91813-149">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="91813-149">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="91813-150">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="91813-150">E.g.</span></span> <span data-ttu-id="91813-151">Die App wird auf einem gerooteten Gerät ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="91813-151">app running on rooted device</span></span>|
|<span data-ttu-id="91813-152">userId</span><span class="sxs-lookup"><span data-stu-id="91813-152">userId</span></span>|<span data-ttu-id="91813-153">String</span><span class="sxs-lookup"><span data-stu-id="91813-153">String</span></span>|<span data-ttu-id="91813-154">Benutzer-ID, zu der die App-Registrierung gehört</span><span class="sxs-lookup"><span data-stu-id="91813-154">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="91813-155">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="91813-155">appIdentifier</span></span>|[<span data-ttu-id="91813-156">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="91813-156">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="91813-157">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="91813-157">The app package Identifier</span></span>|
|<span data-ttu-id="91813-158">id</span><span class="sxs-lookup"><span data-stu-id="91813-158">id</span></span>|<span data-ttu-id="91813-159">String</span><span class="sxs-lookup"><span data-stu-id="91813-159">String</span></span>|<span data-ttu-id="91813-160">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="91813-160">Key of the entity.</span></span>|
|<span data-ttu-id="91813-161">version</span><span class="sxs-lookup"><span data-stu-id="91813-161">version</span></span>|<span data-ttu-id="91813-162">String</span><span class="sxs-lookup"><span data-stu-id="91813-162">String</span></span>|<span data-ttu-id="91813-163">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="91813-163">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91813-164">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="91813-164">Relationships</span></span>
|<span data-ttu-id="91813-165">Beziehung</span><span class="sxs-lookup"><span data-stu-id="91813-165">Relationship</span></span>|<span data-ttu-id="91813-166">Typ</span><span class="sxs-lookup"><span data-stu-id="91813-166">Type</span></span>|<span data-ttu-id="91813-167">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91813-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91813-168">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="91813-168">appliedPolicies</span></span>|<span data-ttu-id="91813-169">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="91813-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="91813-170">Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde</span><span class="sxs-lookup"><span data-stu-id="91813-170">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="91813-171">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="91813-171">intendedPolicies</span></span>|<span data-ttu-id="91813-172">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="91813-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="91813-173">Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat</span><span class="sxs-lookup"><span data-stu-id="91813-173">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="91813-174">operations</span><span class="sxs-lookup"><span data-stu-id="91813-174">operations</span></span>|<span data-ttu-id="91813-175">Sammlung von Objekten des Typs [managedAppOperation](../resources/intune_mam_managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="91813-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) collection</span></span>|<span data-ttu-id="91813-176">Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="91813-176">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91813-177">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91813-177">JSON Representation</span></span>
<span data-ttu-id="91813-178">Unten sehen Sie eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91813-178">Here is a JSON representation of the resource.</span></span>
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
     "Warning: /api-reference/v1.0/resources/intune_mam_managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
