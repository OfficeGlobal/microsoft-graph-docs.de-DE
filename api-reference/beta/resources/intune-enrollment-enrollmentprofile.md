---
title: enrollmentProfile-Ressourcentyp
description: Die enrollmentProfile-Ressource stellt eine Auflistung von Konfigurationen dar, die vor der Registrierung bereitgestellt werden müssen, um die Anmeldung bestimmter Geräte zu ermöglichen, deren Identitäten bereits vorbereitt wurden. Diesem Profiltyp werden Pre-Staging-Geräte Identitäten zugewiesen, um die Konfigurationen des Profils bei der Registrierung des entsprechenden Geräts anzuwenden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d8947864611ac2c0d26256a5d739d41b86c383f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151177"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="3e10f-104">enrollmentProfile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3e10f-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="3e10f-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e10f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e10f-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3e10f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e10f-107">Die enrollmentProfile-Ressource stellt eine Auflistung von Konfigurationen dar, die vor der Registrierung bereitgestellt werden müssen, um die Anmeldung bestimmter Geräte zu ermöglichen, deren Identitäten bereits vorbereitt wurden.</span><span class="sxs-lookup"><span data-stu-id="3e10f-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="3e10f-108">Diesem Profiltyp werden Pre-Staging-Geräte Identitäten zugewiesen, um die Konfigurationen des Profils bei der Registrierung des entsprechenden Geräts anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="3e10f-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="3e10f-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="3e10f-109">Methods</span></span>
|<span data-ttu-id="3e10f-110">Methode</span><span class="sxs-lookup"><span data-stu-id="3e10f-110">Method</span></span>|<span data-ttu-id="3e10f-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3e10f-111">Return Type</span></span>|<span data-ttu-id="3e10f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e10f-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e10f-113">EnrollmentProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="3e10f-113">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="3e10f-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="3e10f-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="3e10f-115">AufListen von Eigenschaften und Beziehungen der [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="3e10f-115">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="3e10f-116">EnrollmentProfile abrufen</span><span class="sxs-lookup"><span data-stu-id="3e10f-116">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="3e10f-117">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3e10f-117">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="3e10f-118">Lesen von Eigenschaften und Beziehungen des [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e10f-118">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="3e10f-119">EnrollmentProfile erstellen</span><span class="sxs-lookup"><span data-stu-id="3e10f-119">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="3e10f-120">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3e10f-120">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="3e10f-121">Erstellen eines neuen [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e10f-121">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="3e10f-122">EnrollmentProfile löschen</span><span class="sxs-lookup"><span data-stu-id="3e10f-122">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="3e10f-123">Keine</span><span class="sxs-lookup"><span data-stu-id="3e10f-123">None</span></span>|<span data-ttu-id="3e10f-124">Löscht eine [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="3e10f-124">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="3e10f-125">EnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3e10f-125">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="3e10f-126">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="3e10f-126">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="3e10f-127">Aktualisieren der Eigenschaften eines [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e10f-127">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="3e10f-128">setDefaultProfile-Aktion</span><span class="sxs-lookup"><span data-stu-id="3e10f-128">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="3e10f-129">Keine</span><span class="sxs-lookup"><span data-stu-id="3e10f-129">None</span></span>|<span data-ttu-id="3e10f-130">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3e10f-130">Not yet documented</span></span>|
|[<span data-ttu-id="3e10f-131">exportMobileConfig-Funktion</span><span class="sxs-lookup"><span data-stu-id="3e10f-131">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="3e10f-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e10f-132">String</span></span>|<span data-ttu-id="3e10f-133">Exportiert die Mobile Konfiguration</span><span class="sxs-lookup"><span data-stu-id="3e10f-133">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="3e10f-134">updateDeviceProfileAssignment-Aktion</span><span class="sxs-lookup"><span data-stu-id="3e10f-134">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="3e10f-135">Keine</span><span class="sxs-lookup"><span data-stu-id="3e10f-135">None</span></span>|<span data-ttu-id="3e10f-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3e10f-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3e10f-137">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3e10f-137">Properties</span></span>
|<span data-ttu-id="3e10f-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e10f-138">Property</span></span>|<span data-ttu-id="3e10f-139">Typ</span><span class="sxs-lookup"><span data-stu-id="3e10f-139">Type</span></span>|<span data-ttu-id="3e10f-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e10f-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e10f-141">id</span><span class="sxs-lookup"><span data-stu-id="3e10f-141">id</span></span>|<span data-ttu-id="3e10f-142">String</span><span class="sxs-lookup"><span data-stu-id="3e10f-142">String</span></span>|<span data-ttu-id="3e10f-143">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="3e10f-143">The GUID for the object</span></span>|
|<span data-ttu-id="3e10f-144">displayName</span><span class="sxs-lookup"><span data-stu-id="3e10f-144">displayName</span></span>|<span data-ttu-id="3e10f-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e10f-145">String</span></span>|<span data-ttu-id="3e10f-146">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="3e10f-146">Name of the profile</span></span>|
|<span data-ttu-id="3e10f-147">description</span><span class="sxs-lookup"><span data-stu-id="3e10f-147">description</span></span>|<span data-ttu-id="3e10f-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e10f-148">String</span></span>|<span data-ttu-id="3e10f-149">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="3e10f-149">Description of the profile</span></span>|
|<span data-ttu-id="3e10f-150">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="3e10f-150">requiresUserAuthentication</span></span>|<span data-ttu-id="3e10f-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3e10f-151">Boolean</span></span>|<span data-ttu-id="3e10f-152">Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert.</span><span class="sxs-lookup"><span data-stu-id="3e10f-152">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="3e10f-153">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="3e10f-153">configurationEndpointUrl</span></span>|<span data-ttu-id="3e10f-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e10f-154">String</span></span>|<span data-ttu-id="3e10f-155">Konfigurations Endpunkt-URL für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="3e10f-155">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="3e10f-156">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="3e10f-156">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="3e10f-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3e10f-157">Boolean</span></span>|<span data-ttu-id="3e10f-158">Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll.</span><span class="sxs-lookup"><span data-stu-id="3e10f-158">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="3e10f-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="3e10f-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="3e10f-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3e10f-160">Boolean</span></span>|<span data-ttu-id="3e10f-161">Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten für registrierte Geräte erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="3e10f-161">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e10f-162">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3e10f-162">Relationships</span></span>
<span data-ttu-id="3e10f-163">Keine</span><span class="sxs-lookup"><span data-stu-id="3e10f-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e10f-164">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3e10f-164">JSON Representation</span></span>
<span data-ttu-id="3e10f-165">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3e10f-165">Here is a JSON representation of the resource.</span></span>
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




