---
title: Ressourcentyp enrollmentProfile
description: Die Ressource EnrollmentProfile stellt eine Auflistung von Konfigurationen, die bereitgestellt werden müssen vor dem Registrierung zum Registrieren von bestimmten Geräten, deren Identitäten vorab bereitgestellt wurden, aktivieren. Provisorisch Gerät Identitäten werden mit diesem Profil zugewiesen, das Profil Konfigurationen zur Registrierung des entsprechenden Geräts angewendet.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b88745c060e71e32199a96b23f94fa0d3229d451
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935591"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="2a14c-104">Ressourcentyp enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="2a14c-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="2a14c-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2a14c-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a14c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a14c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a14c-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2a14c-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a14c-108">Die Ressource EnrollmentProfile stellt eine Auflistung von Konfigurationen, die bereitgestellt werden müssen vor dem Registrierung zum Registrieren von bestimmten Geräten, deren Identitäten vorab bereitgestellt wurden, aktivieren.</span><span class="sxs-lookup"><span data-stu-id="2a14c-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="2a14c-109">Provisorisch Gerät Identitäten werden mit diesem Profil zugewiesen, das Profil Konfigurationen zur Registrierung des entsprechenden Geräts angewendet.</span><span class="sxs-lookup"><span data-stu-id="2a14c-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>
## <a name="methods"></a><span data-ttu-id="2a14c-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="2a14c-110">Methods</span></span>
|<span data-ttu-id="2a14c-111">Methode</span><span class="sxs-lookup"><span data-stu-id="2a14c-111">Method</span></span>|<span data-ttu-id="2a14c-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2a14c-112">Return Type</span></span>|<span data-ttu-id="2a14c-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a14c-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2a14c-114">Liste enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="2a14c-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="2a14c-115">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="2a14c-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="2a14c-116">Listeneigenschaften und Beziehungen der [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="2a14c-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="2a14c-117">Abrufen von enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="2a14c-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="2a14c-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="2a14c-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="2a14c-119">Lesen Sie Eigenschaften und Beziehungen des [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a14c-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="2a14c-120">Erstellen von enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="2a14c-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="2a14c-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="2a14c-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="2a14c-122">Erstellen eines neuen [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a14c-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="2a14c-123">EnrollmentProfile löschen</span><span class="sxs-lookup"><span data-stu-id="2a14c-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="2a14c-124">Keine</span><span class="sxs-lookup"><span data-stu-id="2a14c-124">None</span></span>|<span data-ttu-id="2a14c-125">Löscht eine [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="2a14c-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="2a14c-126">EnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2a14c-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="2a14c-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="2a14c-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="2a14c-128">Aktualisieren Sie die Eigenschaften eines [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a14c-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="2a14c-129">SetDefaultProfile Aktion</span><span class="sxs-lookup"><span data-stu-id="2a14c-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="2a14c-130">Keine</span><span class="sxs-lookup"><span data-stu-id="2a14c-130">None</span></span>|<span data-ttu-id="2a14c-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2a14c-131">Not yet documented</span></span>|
|[<span data-ttu-id="2a14c-132">ExportMobileConfig-Funktion</span><span class="sxs-lookup"><span data-stu-id="2a14c-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="2a14c-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a14c-133">String</span></span>|<span data-ttu-id="2a14c-134">Exportiert die mobile Konfiguration</span><span class="sxs-lookup"><span data-stu-id="2a14c-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="2a14c-135">UpdateDeviceProfileAssignment Aktion</span><span class="sxs-lookup"><span data-stu-id="2a14c-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="2a14c-136">Keine</span><span class="sxs-lookup"><span data-stu-id="2a14c-136">None</span></span>|<span data-ttu-id="2a14c-137">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2a14c-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2a14c-138">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2a14c-138">Properties</span></span>
|<span data-ttu-id="2a14c-139">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a14c-139">Property</span></span>|<span data-ttu-id="2a14c-140">Typ</span><span class="sxs-lookup"><span data-stu-id="2a14c-140">Type</span></span>|<span data-ttu-id="2a14c-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a14c-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a14c-142">id</span><span class="sxs-lookup"><span data-stu-id="2a14c-142">id</span></span>|<span data-ttu-id="2a14c-143">String</span><span class="sxs-lookup"><span data-stu-id="2a14c-143">String</span></span>|<span data-ttu-id="2a14c-144">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="2a14c-144">The GUID for the object</span></span>|
|<span data-ttu-id="2a14c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="2a14c-145">displayName</span></span>|<span data-ttu-id="2a14c-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a14c-146">String</span></span>|<span data-ttu-id="2a14c-147">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="2a14c-147">Name of the profile</span></span>|
|<span data-ttu-id="2a14c-148">description</span><span class="sxs-lookup"><span data-stu-id="2a14c-148">description</span></span>|<span data-ttu-id="2a14c-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a14c-149">String</span></span>|<span data-ttu-id="2a14c-150">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="2a14c-150">Description of the profile</span></span>|
|<span data-ttu-id="2a14c-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="2a14c-151">requiresUserAuthentication</span></span>|<span data-ttu-id="2a14c-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2a14c-152">Boolean</span></span>|<span data-ttu-id="2a14c-153">Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert</span><span class="sxs-lookup"><span data-stu-id="2a14c-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="2a14c-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="2a14c-154">configurationEndpointUrl</span></span>|<span data-ttu-id="2a14c-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a14c-155">String</span></span>|<span data-ttu-id="2a14c-156">Endpunkt-Url für die Registrierung zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="2a14c-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="2a14c-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="2a14c-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="2a14c-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2a14c-158">Boolean</span></span>|<span data-ttu-id="2a14c-159">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="2a14c-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a14c-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2a14c-160">Relationships</span></span>
<span data-ttu-id="2a14c-161">Keine</span><span class="sxs-lookup"><span data-stu-id="2a14c-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a14c-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2a14c-162">JSON Representation</span></span>
<span data-ttu-id="2a14c-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a14c-163">Here is a JSON representation of the resource.</span></span>
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





