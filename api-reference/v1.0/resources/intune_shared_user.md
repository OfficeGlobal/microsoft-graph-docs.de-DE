# <a name="user-resource-type"></a><span data-ttu-id="d7e2c-101">user-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d7e2c-101">user resource type</span></span>

> <span data-ttu-id="d7e2c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7e2c-103">Stellt ein user-Objekt von Azure Active Directory dar.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-103">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="d7e2c-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="d7e2c-104">Methods</span></span>
|<span data-ttu-id="d7e2c-105">Methode</span><span class="sxs-lookup"><span data-stu-id="d7e2c-105">Method</span></span>|<span data-ttu-id="d7e2c-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d7e2c-106">Return Type</span></span>|<span data-ttu-id="d7e2c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7e2c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7e2c-108">[Benutzer auflisten](../api/intune_shared_user_list.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-108">[List users](../api/intune_shared_user_list.md) objects.</span></span>|
|<span data-ttu-id="d7e2c-109">[Benutzer abrufen](../api/intune_shared_user_get.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-109">[Get user](../api/intune_shared_user_get.md) object.</span></span>|
|<span data-ttu-id="d7e2c-110">[Benutzer erstellen](../api/intune_shared_user_create.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-110">Create a new [user](../api/intune_shared_user_create.md) object.</span></span>|
|<span data-ttu-id="d7e2c-111">[Benutzer löschen](../api/intune_shared_user_delete.md).</span><span class="sxs-lookup"><span data-stu-id="d7e2c-111">Delete user</span></span>|
|<span data-ttu-id="d7e2c-112">[Benutzer aktualisieren](../api/intune_shared_user_update.md)-Benutzerobjekt.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-112">Update user object.</span></span>|
|<span data-ttu-id="d7e2c-113">**Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="d7e2c-113">**Device management**</span></span>|
|[<span data-ttu-id="d7e2c-114">removeAllDevicesFromManagement-Aktion</span><span class="sxs-lookup"><span data-stu-id="d7e2c-114">removeAllDevicesFromManagement action</span></span>](../api/intune_shared_user_removealldevicesfrommanagement.md)|<span data-ttu-id="d7e2c-115">Keine</span><span class="sxs-lookup"><span data-stu-id="d7e2c-115">None</span></span>|<span data-ttu-id="d7e2c-116">Die Verwaltung aller Geräte für diesen Benutzer außer Kraft setzen</span><span class="sxs-lookup"><span data-stu-id="d7e2c-116">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="d7e2c-117">**Mobile Anwendungsverwaltung (MAM)**</span><span class="sxs-lookup"><span data-stu-id="d7e2c-117">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="d7e2c-118">getManagedAppDiagnosticStatuses-Funktion</span><span class="sxs-lookup"><span data-stu-id="d7e2c-118">getManagedAppDiagnosticStatuses function</span></span>](../api/intune_shared_user_getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="d7e2c-119">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d7e2c-119">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="d7e2c-120">Ruft den Status der Diagnoseüberprüfung für einen bestimmten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-120">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="d7e2c-121">getManagedAppPolicies-Funktion</span><span class="sxs-lookup"><span data-stu-id="d7e2c-121">getManagedAppPolicies function</span></span>](../api/intune_shared_user_getmanagedapppolicies.md)|<span data-ttu-id="d7e2c-122">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d7e2c-122">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="d7e2c-123">Ruft App-Einschränkungen für einen bestimmten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-123">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="d7e2c-124">wipeManagedAppRegistrationsByDeviceTag-Aktion</span><span class="sxs-lookup"><span data-stu-id="d7e2c-124">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune_shared_user_wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="d7e2c-125">Keine</span><span class="sxs-lookup"><span data-stu-id="d7e2c-125">None</span></span>|<span data-ttu-id="d7e2c-126">Gibt einen Zurücksetzungsvorgang für eine App-Registrierung mit angegebenem Geräte-Tag aus.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-126">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7e2c-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d7e2c-127">Properties</span></span>
|<span data-ttu-id="d7e2c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d7e2c-128">Property</span></span>|<span data-ttu-id="d7e2c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d7e2c-129">Type</span></span>|<span data-ttu-id="d7e2c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7e2c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7e2c-131">ID</span><span class="sxs-lookup"><span data-stu-id="d7e2c-131">id</span></span>|<span data-ttu-id="d7e2c-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d7e2c-132">String</span></span>|<span data-ttu-id="d7e2c-133">Eindeutiger Bezeichner des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-133">Unique identifier of the user.</span></span>|
|<span data-ttu-id="d7e2c-134">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="d7e2c-134">**On-boarding**</span></span>|
|<span data-ttu-id="d7e2c-135">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="d7e2c-135">deviceEnrollmentLimit</span></span>|<span data-ttu-id="d7e2c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d7e2c-136">Int32</span></span>|<span data-ttu-id="d7e2c-137">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-137">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="d7e2c-138">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-138">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d7e2c-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d7e2c-139">Relationships</span></span>
|<span data-ttu-id="d7e2c-140">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d7e2c-140">Relationship</span></span>|<span data-ttu-id="d7e2c-141">Typ</span><span class="sxs-lookup"><span data-stu-id="d7e2c-141">Type</span></span>|<span data-ttu-id="d7e2c-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7e2c-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7e2c-143">**Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="d7e2c-143">**Device management**</span></span>|
|<span data-ttu-id="d7e2c-144">managedDevices</span><span class="sxs-lookup"><span data-stu-id="d7e2c-144">managedDevices</span></span>|<span data-ttu-id="d7e2c-145">[managedDevice](../resources/intune_devices_manageddevice.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d7e2c-145">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="d7e2c-146">Die mit dem Benutzer verknüpften verwalteten Geräte.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-146">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="d7e2c-147">**Mobile Anwendungsverwaltung (MAM)**</span><span class="sxs-lookup"><span data-stu-id="d7e2c-147">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="d7e2c-148">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="d7e2c-148">managedAppRegistrations</span></span>|<span data-ttu-id="d7e2c-149">[managedAppRegistration](../resources/intune_mam_managedappregistration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d7e2c-149">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="d7e2c-150">Null oder mehr verwaltete App-Registrierungen, die dem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-150">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="d7e2c-151">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="d7e2c-151">**Troubleshooting**</span></span>|
|<span data-ttu-id="d7e2c-152">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="d7e2c-152">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="d7e2c-153">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d7e2c-153">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="d7e2c-154">Die Liste der Problembehandlungsereignisse für diesen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-154">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7e2c-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d7e2c-155">JSON Representation</span></span>
<span data-ttu-id="d7e2c-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d7e2c-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
