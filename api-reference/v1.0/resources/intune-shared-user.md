---
title: user-Ressourcentyp
description: Stellt ein user-Objekt von Azure Active Directory dar.
ms.openlocfilehash: 5d1d8e18e120fb26cfd5cea1cd223a6c38ad0aa9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018662"
---
# <a name="user-resource-type"></a><span data-ttu-id="1758e-103">user-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1758e-103">user resource type</span></span>

> <span data-ttu-id="1758e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1758e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1758e-105">Stellt ein user-Objekt von Azure Active Directory dar.</span><span class="sxs-lookup"><span data-stu-id="1758e-105">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="1758e-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="1758e-106">Methods</span></span>
|<span data-ttu-id="1758e-107">Methode</span><span class="sxs-lookup"><span data-stu-id="1758e-107">Method</span></span>|<span data-ttu-id="1758e-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1758e-108">Return Type</span></span>|<span data-ttu-id="1758e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1758e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1758e-110">[Liste Benutzer](../api/intune-shared-user-list.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="1758e-110">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="1758e-111">[user](../resources/intune-shared-user.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1758e-111">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="1758e-112">Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune-shared-user.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="1758e-112">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="1758e-113">[Abrufen von Benutzer](../api/intune-shared-user-get.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="1758e-113">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="1758e-114">[Benutzersammlung](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="1758e-114">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="1758e-115">Lesen von Eigenschaften und Beziehungen des [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1758e-115">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="1758e-116">[Create User](../api/intune-shared-user-create.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="1758e-116">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="1758e-117">[Benutzersammlung](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="1758e-117">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="1758e-118">Dient zum Erstellen eines neuen [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1758e-118">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="1758e-119">[Benutzer löschen](../api/intune-shared-user-delete.md).</span><span class="sxs-lookup"><span data-stu-id="1758e-119">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="1758e-120">Keine</span><span class="sxs-lookup"><span data-stu-id="1758e-120">None</span></span>|<span data-ttu-id="1758e-121">Löscht einen [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="1758e-121">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="1758e-122">[Update](../api/intune-shared-user-update.md) -Benutzerobjekt.</span><span class="sxs-lookup"><span data-stu-id="1758e-122">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="1758e-123">user</span><span class="sxs-lookup"><span data-stu-id="1758e-123">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="1758e-124">Aktualisieren der Eigenschaften eines [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1758e-124">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="1758e-125">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="1758e-125">**Device management**</span></span>|
|[<span data-ttu-id="1758e-126">removeAllDevicesFromManagement-Aktion</span><span class="sxs-lookup"><span data-stu-id="1758e-126">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="1758e-127">Keine</span><span class="sxs-lookup"><span data-stu-id="1758e-127">None</span></span>|<span data-ttu-id="1758e-128">Die Verwaltung aller Geräte für diesen Benutzer einstellen.</span><span class="sxs-lookup"><span data-stu-id="1758e-128">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="1758e-129">**Mobile app-Verwaltung (MAM)**</span><span class="sxs-lookup"><span data-stu-id="1758e-129">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="1758e-130">getManagedAppDiagnosticStatuses-Funktion</span><span class="sxs-lookup"><span data-stu-id="1758e-130">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="1758e-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1758e-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="1758e-132">Ruft den Status der Diagnoseüberprüfung für einen bestimmten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="1758e-132">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="1758e-133">getManagedAppPolicies-Funktion</span><span class="sxs-lookup"><span data-stu-id="1758e-133">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="1758e-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1758e-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="1758e-135">Ruft App-Einschränkungen für einen bestimmten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="1758e-135">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="1758e-136">wipeManagedAppRegistrationsByDeviceTag-Aktion</span><span class="sxs-lookup"><span data-stu-id="1758e-136">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="1758e-137">Keine</span><span class="sxs-lookup"><span data-stu-id="1758e-137">None</span></span>|<span data-ttu-id="1758e-138">Gibt einen Zurücksetzungsvorgang für eine App-Registrierung mit angegebenem Geräte-Tag aus.</span><span class="sxs-lookup"><span data-stu-id="1758e-138">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="1758e-139">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1758e-139">Properties</span></span>
|<span data-ttu-id="1758e-140">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1758e-140">Property</span></span>|<span data-ttu-id="1758e-141">Typ</span><span class="sxs-lookup"><span data-stu-id="1758e-141">Type</span></span>|<span data-ttu-id="1758e-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1758e-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1758e-143">id</span><span class="sxs-lookup"><span data-stu-id="1758e-143">id</span></span>|<span data-ttu-id="1758e-144">String</span><span class="sxs-lookup"><span data-stu-id="1758e-144">String</span></span>|<span data-ttu-id="1758e-145">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="1758e-145">Unique identifier of the user.</span></span>|
|<span data-ttu-id="1758e-146">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="1758e-146">**Onboarding**</span></span>|
|<span data-ttu-id="1758e-147">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="1758e-147">deviceEnrollmentLimit</span></span>|<span data-ttu-id="1758e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1758e-148">Int32</span></span>|<span data-ttu-id="1758e-149">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="1758e-149">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="1758e-150">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="1758e-150">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1758e-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1758e-151">Relationships</span></span>
|<span data-ttu-id="1758e-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1758e-152">Relationship</span></span>|<span data-ttu-id="1758e-153">Typ</span><span class="sxs-lookup"><span data-stu-id="1758e-153">Type</span></span>|<span data-ttu-id="1758e-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1758e-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1758e-155">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="1758e-155">**Device management**</span></span>|
|<span data-ttu-id="1758e-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="1758e-156">managedDevices</span></span>|<span data-ttu-id="1758e-157">[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1758e-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="1758e-158">Die mit dem Benutzer verknüpften verwalteten Geräte.</span><span class="sxs-lookup"><span data-stu-id="1758e-158">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="1758e-159">**Mobile app-Verwaltung (MAM)**</span><span class="sxs-lookup"><span data-stu-id="1758e-159">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="1758e-160">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="1758e-160">managedAppRegistrations</span></span>|<span data-ttu-id="1758e-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1758e-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="1758e-162">Null oder mehr verwaltete App-Registrierungen, die dem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="1758e-162">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="1758e-163">**Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="1758e-163">**Troubleshooting**</span></span>|
|<span data-ttu-id="1758e-164">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="1758e-164">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="1758e-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1758e-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="1758e-166">Die Liste der Problembehandlungsereignisse für diesen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="1758e-166">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1758e-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1758e-167">JSON Representation</span></span>
<span data-ttu-id="1758e-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1758e-168">Here is a JSON representation of the resource.</span></span>
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
