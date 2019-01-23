---
title: Ressourcentyp enrollmentProfile
description: Die Ressource EnrollmentProfile stellt eine Auflistung von Konfigurationen, die bereitgestellt werden müssen vor dem Registrierung zum Registrieren von bestimmten Geräten, deren Identitäten vorab bereitgestellt wurden, aktivieren. Provisorisch Gerät Identitäten werden mit diesem Profil zugewiesen, das Profil Konfigurationen zur Registrierung des entsprechenden Geräts angewendet.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a7ce4aac1e22610d539419dd6a63d124616b83f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396840"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="065aa-104">Ressourcentyp enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="065aa-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="065aa-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="065aa-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="065aa-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="065aa-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="065aa-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="065aa-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="065aa-108">Die Ressource EnrollmentProfile stellt eine Auflistung von Konfigurationen, die bereitgestellt werden müssen vor dem Registrierung zum Registrieren von bestimmten Geräten, deren Identitäten vorab bereitgestellt wurden, aktivieren.</span><span class="sxs-lookup"><span data-stu-id="065aa-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="065aa-109">Provisorisch Gerät Identitäten werden mit diesem Profil zugewiesen, das Profil Konfigurationen zur Registrierung des entsprechenden Geräts angewendet.</span><span class="sxs-lookup"><span data-stu-id="065aa-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="065aa-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="065aa-110">Methods</span></span>
|<span data-ttu-id="065aa-111">Methode</span><span class="sxs-lookup"><span data-stu-id="065aa-111">Method</span></span>|<span data-ttu-id="065aa-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="065aa-112">Return Type</span></span>|<span data-ttu-id="065aa-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="065aa-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="065aa-114">Liste enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="065aa-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="065aa-115">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="065aa-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="065aa-116">Listeneigenschaften und Beziehungen der [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="065aa-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="065aa-117">Abrufen von enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="065aa-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="065aa-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="065aa-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="065aa-119">Lesen Sie Eigenschaften und Beziehungen des [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="065aa-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="065aa-120">Erstellen von enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="065aa-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="065aa-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="065aa-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="065aa-122">Erstellen eines neuen [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="065aa-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="065aa-123">EnrollmentProfile löschen</span><span class="sxs-lookup"><span data-stu-id="065aa-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="065aa-124">Keine</span><span class="sxs-lookup"><span data-stu-id="065aa-124">None</span></span>|<span data-ttu-id="065aa-125">Löscht eine [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="065aa-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="065aa-126">EnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="065aa-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="065aa-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="065aa-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="065aa-128">Aktualisieren Sie die Eigenschaften eines [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="065aa-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="065aa-129">SetDefaultProfile Aktion</span><span class="sxs-lookup"><span data-stu-id="065aa-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="065aa-130">Keine</span><span class="sxs-lookup"><span data-stu-id="065aa-130">None</span></span>|<span data-ttu-id="065aa-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="065aa-131">Not yet documented</span></span>|
|[<span data-ttu-id="065aa-132">ExportMobileConfig-Funktion</span><span class="sxs-lookup"><span data-stu-id="065aa-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="065aa-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065aa-133">String</span></span>|<span data-ttu-id="065aa-134">Exportiert die mobile Konfiguration</span><span class="sxs-lookup"><span data-stu-id="065aa-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="065aa-135">UpdateDeviceProfileAssignment Aktion</span><span class="sxs-lookup"><span data-stu-id="065aa-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="065aa-136">Keine</span><span class="sxs-lookup"><span data-stu-id="065aa-136">None</span></span>|<span data-ttu-id="065aa-137">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="065aa-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="065aa-138">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="065aa-138">Properties</span></span>
|<span data-ttu-id="065aa-139">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="065aa-139">Property</span></span>|<span data-ttu-id="065aa-140">Typ</span><span class="sxs-lookup"><span data-stu-id="065aa-140">Type</span></span>|<span data-ttu-id="065aa-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="065aa-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="065aa-142">id</span><span class="sxs-lookup"><span data-stu-id="065aa-142">id</span></span>|<span data-ttu-id="065aa-143">String</span><span class="sxs-lookup"><span data-stu-id="065aa-143">String</span></span>|<span data-ttu-id="065aa-144">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="065aa-144">The GUID for the object</span></span>|
|<span data-ttu-id="065aa-145">displayName</span><span class="sxs-lookup"><span data-stu-id="065aa-145">displayName</span></span>|<span data-ttu-id="065aa-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065aa-146">String</span></span>|<span data-ttu-id="065aa-147">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="065aa-147">Name of the profile</span></span>|
|<span data-ttu-id="065aa-148">description</span><span class="sxs-lookup"><span data-stu-id="065aa-148">description</span></span>|<span data-ttu-id="065aa-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065aa-149">String</span></span>|<span data-ttu-id="065aa-150">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="065aa-150">Description of the profile</span></span>|
|<span data-ttu-id="065aa-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="065aa-151">requiresUserAuthentication</span></span>|<span data-ttu-id="065aa-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="065aa-152">Boolean</span></span>|<span data-ttu-id="065aa-153">Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert</span><span class="sxs-lookup"><span data-stu-id="065aa-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="065aa-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="065aa-154">configurationEndpointUrl</span></span>|<span data-ttu-id="065aa-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="065aa-155">String</span></span>|<span data-ttu-id="065aa-156">Endpunkt-Url für die Registrierung zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="065aa-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="065aa-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="065aa-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="065aa-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="065aa-158">Boolean</span></span>|<span data-ttu-id="065aa-159">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="065aa-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="065aa-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="065aa-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="065aa-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="065aa-161">Boolean</span></span>|<span data-ttu-id="065aa-162">Gibt an, dass Unternehmensportal auf Setup-Assistent registriert Geräten erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="065aa-162">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="065aa-163">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="065aa-163">Relationships</span></span>
<span data-ttu-id="065aa-164">Keine</span><span class="sxs-lookup"><span data-stu-id="065aa-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="065aa-165">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="065aa-165">JSON Representation</span></span>
<span data-ttu-id="065aa-166">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="065aa-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




