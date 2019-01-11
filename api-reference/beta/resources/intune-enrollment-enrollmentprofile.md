---
title: Ressourcentyp enrollmentProfile
description: Die Ressource EnrollmentProfile stellt eine Auflistung von Konfigurationen, die bereitgestellt werden müssen vor dem Registrierung zum Registrieren von bestimmten Geräten, deren Identitäten vorab bereitgestellt wurden, aktivieren. Provisorisch Gerät Identitäten werden mit diesem Profil zugewiesen, das Profil Konfigurationen zur Registrierung des entsprechenden Geräts angewendet.
localization_priority: Normal
ms.openlocfilehash: 43aa6f5f3e8093da0c066012d763e5f0f6455da6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894306"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="c7443-104">Ressourcentyp enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c7443-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="c7443-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c7443-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7443-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7443-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7443-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c7443-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7443-108">Die Ressource EnrollmentProfile stellt eine Auflistung von Konfigurationen, die bereitgestellt werden müssen vor dem Registrierung zum Registrieren von bestimmten Geräten, deren Identitäten vorab bereitgestellt wurden, aktivieren.</span><span class="sxs-lookup"><span data-stu-id="c7443-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="c7443-109">Provisorisch Gerät Identitäten werden mit diesem Profil zugewiesen, das Profil Konfigurationen zur Registrierung des entsprechenden Geräts angewendet.</span><span class="sxs-lookup"><span data-stu-id="c7443-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>
## <a name="methods"></a><span data-ttu-id="c7443-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="c7443-110">Methods</span></span>
|<span data-ttu-id="c7443-111">Methode</span><span class="sxs-lookup"><span data-stu-id="c7443-111">Method</span></span>|<span data-ttu-id="c7443-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c7443-112">Return Type</span></span>|<span data-ttu-id="c7443-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7443-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7443-114">Liste enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="c7443-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="c7443-115">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c7443-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="c7443-116">Listeneigenschaften und Beziehungen der [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="c7443-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="c7443-117">Abrufen von enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c7443-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="c7443-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c7443-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="c7443-119">Lesen Sie Eigenschaften und Beziehungen des [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7443-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="c7443-120">Erstellen von enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c7443-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="c7443-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c7443-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="c7443-122">Erstellen eines neuen [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7443-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="c7443-123">EnrollmentProfile löschen</span><span class="sxs-lookup"><span data-stu-id="c7443-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="c7443-124">Keine</span><span class="sxs-lookup"><span data-stu-id="c7443-124">None</span></span>|<span data-ttu-id="c7443-125">Löscht eine [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c7443-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="c7443-126">EnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c7443-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="c7443-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c7443-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="c7443-128">Aktualisieren Sie die Eigenschaften eines [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7443-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="c7443-129">SetDefaultProfile Aktion</span><span class="sxs-lookup"><span data-stu-id="c7443-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="c7443-130">Keine</span><span class="sxs-lookup"><span data-stu-id="c7443-130">None</span></span>|<span data-ttu-id="c7443-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c7443-131">Not yet documented</span></span>|
|[<span data-ttu-id="c7443-132">ExportMobileConfig-Funktion</span><span class="sxs-lookup"><span data-stu-id="c7443-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="c7443-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7443-133">String</span></span>|<span data-ttu-id="c7443-134">Exportiert die mobile Konfiguration</span><span class="sxs-lookup"><span data-stu-id="c7443-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="c7443-135">UpdateDeviceProfileAssignment Aktion</span><span class="sxs-lookup"><span data-stu-id="c7443-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="c7443-136">Keine</span><span class="sxs-lookup"><span data-stu-id="c7443-136">None</span></span>|<span data-ttu-id="c7443-137">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c7443-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c7443-138">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7443-138">Properties</span></span>
|<span data-ttu-id="c7443-139">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7443-139">Property</span></span>|<span data-ttu-id="c7443-140">Typ</span><span class="sxs-lookup"><span data-stu-id="c7443-140">Type</span></span>|<span data-ttu-id="c7443-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7443-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7443-142">id</span><span class="sxs-lookup"><span data-stu-id="c7443-142">id</span></span>|<span data-ttu-id="c7443-143">String</span><span class="sxs-lookup"><span data-stu-id="c7443-143">String</span></span>|<span data-ttu-id="c7443-144">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="c7443-144">The GUID for the object</span></span>|
|<span data-ttu-id="c7443-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c7443-145">displayName</span></span>|<span data-ttu-id="c7443-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7443-146">String</span></span>|<span data-ttu-id="c7443-147">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="c7443-147">Name of the profile</span></span>|
|<span data-ttu-id="c7443-148">description</span><span class="sxs-lookup"><span data-stu-id="c7443-148">description</span></span>|<span data-ttu-id="c7443-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7443-149">String</span></span>|<span data-ttu-id="c7443-150">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="c7443-150">Description of the profile</span></span>|
|<span data-ttu-id="c7443-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="c7443-151">requiresUserAuthentication</span></span>|<span data-ttu-id="c7443-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c7443-152">Boolean</span></span>|<span data-ttu-id="c7443-153">Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert</span><span class="sxs-lookup"><span data-stu-id="c7443-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="c7443-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="c7443-154">configurationEndpointUrl</span></span>|<span data-ttu-id="c7443-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7443-155">String</span></span>|<span data-ttu-id="c7443-156">Endpunkt-Url für die Registrierung zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="c7443-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="c7443-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="c7443-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="c7443-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c7443-158">Boolean</span></span>|<span data-ttu-id="c7443-159">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="c7443-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7443-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c7443-160">Relationships</span></span>
<span data-ttu-id="c7443-161">Keine</span><span class="sxs-lookup"><span data-stu-id="c7443-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7443-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7443-162">JSON Representation</span></span>
<span data-ttu-id="c7443-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7443-163">Here is a JSON representation of the resource.</span></span>
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
  "enableAuthenticationViaCompanyPortal": true
}
```





