---
title: Erstellen von enrollmentProfile
description: Erstellen eines neuen EnrollmentProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a7bb3fb49b57f38ad938f7d43f28f4ece3fda92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414767"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="bbaa6-103">Erstellen von enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bbaa6-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="bbaa6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bbaa6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bbaa6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bbaa6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbaa6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bbaa6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbaa6-107">Erstellen eines neuen [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bbaa6-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbaa6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bbaa6-108">Prerequisites</span></span>
<span data-ttu-id="bbaa6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bbaa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bbaa6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bbaa6-111">Permission type</span></span>|<span data-ttu-id="bbaa6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bbaa6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbaa6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bbaa6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbaa6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbaa6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bbaa6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bbaa6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbaa6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bbaa6-116">Not supported.</span></span>|
|<span data-ttu-id="bbaa6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bbaa6-117">Application</span></span>|<span data-ttu-id="bbaa6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bbaa6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbaa6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bbaa6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="bbaa6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bbaa6-120">Request headers</span></span>
|<span data-ttu-id="bbaa6-121">Header</span><span class="sxs-lookup"><span data-stu-id="bbaa6-121">Header</span></span>|<span data-ttu-id="bbaa6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bbaa6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbaa6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="bbaa6-123">Authorization</span></span>|<span data-ttu-id="bbaa6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bbaa6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbaa6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bbaa6-125">Accept</span></span>|<span data-ttu-id="bbaa6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbaa6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbaa6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bbaa6-127">Request body</span></span>
<span data-ttu-id="bbaa6-128">Geben Sie im Textkörper Anforderung für das Objekt EnrollmentProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="bbaa6-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="bbaa6-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die EnrollmentProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="bbaa6-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="bbaa6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bbaa6-130">Property</span></span>|<span data-ttu-id="bbaa6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bbaa6-131">Type</span></span>|<span data-ttu-id="bbaa6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbaa6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbaa6-133">id</span><span class="sxs-lookup"><span data-stu-id="bbaa6-133">id</span></span>|<span data-ttu-id="bbaa6-134">String</span><span class="sxs-lookup"><span data-stu-id="bbaa6-134">String</span></span>|<span data-ttu-id="bbaa6-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="bbaa6-135">The GUID for the object</span></span>|
|<span data-ttu-id="bbaa6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bbaa6-136">displayName</span></span>|<span data-ttu-id="bbaa6-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bbaa6-137">String</span></span>|<span data-ttu-id="bbaa6-138">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="bbaa6-138">Name of the profile</span></span>|
|<span data-ttu-id="bbaa6-139">description</span><span class="sxs-lookup"><span data-stu-id="bbaa6-139">description</span></span>|<span data-ttu-id="bbaa6-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bbaa6-140">String</span></span>|<span data-ttu-id="bbaa6-141">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="bbaa6-141">Description of the profile</span></span>|
|<span data-ttu-id="bbaa6-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="bbaa6-142">requiresUserAuthentication</span></span>|<span data-ttu-id="bbaa6-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbaa6-143">Boolean</span></span>|<span data-ttu-id="bbaa6-144">Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert</span><span class="sxs-lookup"><span data-stu-id="bbaa6-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="bbaa6-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="bbaa6-145">configurationEndpointUrl</span></span>|<span data-ttu-id="bbaa6-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bbaa6-146">String</span></span>|<span data-ttu-id="bbaa6-147">Endpunkt-Url für die Registrierung zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="bbaa6-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="bbaa6-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="bbaa6-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="bbaa6-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbaa6-149">Boolean</span></span>|<span data-ttu-id="bbaa6-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="bbaa6-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="bbaa6-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="bbaa6-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="bbaa6-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbaa6-152">Boolean</span></span>|<span data-ttu-id="bbaa6-153">Gibt an, dass Unternehmensportal auf Setup-Assistent registriert Geräten erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="bbaa6-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="bbaa6-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="bbaa6-154">Response</span></span>
<span data-ttu-id="bbaa6-155">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bbaa6-155">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbaa6-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bbaa6-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbaa6-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bbaa6-157">Request</span></span>
<span data-ttu-id="bbaa6-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bbaa6-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="bbaa6-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="bbaa6-159">Response</span></span>
<span data-ttu-id="bbaa6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bbaa6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




