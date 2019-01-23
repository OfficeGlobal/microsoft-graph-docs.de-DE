---
title: EnrollmentProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines EnrollmentProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 85cceaaaaa66822340539c38f6ab8ecde88eae1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400739"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="8fdc4-103">EnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8fdc4-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="8fdc4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8fdc4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8fdc4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8fdc4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fdc4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8fdc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fdc4-107">Aktualisieren Sie die Eigenschaften eines [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8fdc4-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fdc4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8fdc4-108">Prerequisites</span></span>
<span data-ttu-id="8fdc4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8fdc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8fdc4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8fdc4-111">Permission type</span></span>|<span data-ttu-id="8fdc4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8fdc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fdc4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8fdc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fdc4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fdc4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8fdc4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8fdc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fdc4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fdc4-116">Not supported.</span></span>|
|<span data-ttu-id="8fdc4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8fdc4-117">Application</span></span>|<span data-ttu-id="8fdc4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fdc4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fdc4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fdc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="8fdc4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8fdc4-120">Request headers</span></span>
|<span data-ttu-id="8fdc4-121">Header</span><span class="sxs-lookup"><span data-stu-id="8fdc4-121">Header</span></span>|<span data-ttu-id="8fdc4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8fdc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fdc4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8fdc4-123">Authorization</span></span>|<span data-ttu-id="8fdc4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8fdc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fdc4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8fdc4-125">Accept</span></span>|<span data-ttu-id="8fdc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fdc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fdc4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8fdc4-127">Request body</span></span>
<span data-ttu-id="8fdc4-128">Geben Sie im Textkörper Anforderung für das Objekt [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8fdc4-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="8fdc4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="8fdc4-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="8fdc4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8fdc4-130">Property</span></span>|<span data-ttu-id="8fdc4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8fdc4-131">Type</span></span>|<span data-ttu-id="8fdc4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fdc4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fdc4-133">id</span><span class="sxs-lookup"><span data-stu-id="8fdc4-133">id</span></span>|<span data-ttu-id="8fdc4-134">String</span><span class="sxs-lookup"><span data-stu-id="8fdc4-134">String</span></span>|<span data-ttu-id="8fdc4-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="8fdc4-135">The GUID for the object</span></span>|
|<span data-ttu-id="8fdc4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8fdc4-136">displayName</span></span>|<span data-ttu-id="8fdc4-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fdc4-137">String</span></span>|<span data-ttu-id="8fdc4-138">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="8fdc4-138">Name of the profile</span></span>|
|<span data-ttu-id="8fdc4-139">description</span><span class="sxs-lookup"><span data-stu-id="8fdc4-139">description</span></span>|<span data-ttu-id="8fdc4-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fdc4-140">String</span></span>|<span data-ttu-id="8fdc4-141">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="8fdc4-141">Description of the profile</span></span>|
|<span data-ttu-id="8fdc4-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="8fdc4-142">requiresUserAuthentication</span></span>|<span data-ttu-id="8fdc4-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fdc4-143">Boolean</span></span>|<span data-ttu-id="8fdc4-144">Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert</span><span class="sxs-lookup"><span data-stu-id="8fdc4-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="8fdc4-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="8fdc4-145">configurationEndpointUrl</span></span>|<span data-ttu-id="8fdc4-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fdc4-146">String</span></span>|<span data-ttu-id="8fdc4-147">Endpunkt-Url für die Registrierung zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="8fdc4-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="8fdc4-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="8fdc4-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="8fdc4-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fdc4-149">Boolean</span></span>|<span data-ttu-id="8fdc4-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="8fdc4-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="8fdc4-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="8fdc4-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="8fdc4-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fdc4-152">Boolean</span></span>|<span data-ttu-id="8fdc4-153">Gibt an, dass Unternehmensportal auf Setup-Assistent registriert Geräten erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="8fdc4-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="8fdc4-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fdc4-154">Response</span></span>
<span data-ttu-id="8fdc4-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8fdc4-155">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fdc4-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8fdc4-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fdc4-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fdc4-157">Request</span></span>
<span data-ttu-id="8fdc4-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8fdc4-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 370

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```

### <a name="response"></a><span data-ttu-id="8fdc4-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fdc4-159">Response</span></span>
<span data-ttu-id="8fdc4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8fdc4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 419

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




