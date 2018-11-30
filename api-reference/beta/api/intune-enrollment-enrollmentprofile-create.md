---
title: Erstellen von enrollmentProfile
description: Erstellen eines neuen EnrollmentProfile-Objekts.
ms.openlocfilehash: 8b24964413250e9a0f9d8d98577e930e1ef99b84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062450"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="95382-103">Erstellen von enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="95382-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="95382-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="95382-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95382-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="95382-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95382-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="95382-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95382-107">Erstellen eines neuen [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="95382-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95382-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="95382-108">Prerequisites</span></span>
<span data-ttu-id="95382-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95382-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95382-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="95382-111">Permission type</span></span>|<span data-ttu-id="95382-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="95382-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95382-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="95382-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95382-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95382-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="95382-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="95382-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95382-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="95382-116">Not supported.</span></span>|
|<span data-ttu-id="95382-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="95382-117">Application</span></span>|<span data-ttu-id="95382-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="95382-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95382-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="95382-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="95382-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="95382-120">Request headers</span></span>
|<span data-ttu-id="95382-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="95382-121">Header</span></span>|<span data-ttu-id="95382-122">Wert</span><span class="sxs-lookup"><span data-stu-id="95382-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95382-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95382-123">Authorization</span></span>|<span data-ttu-id="95382-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="95382-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95382-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95382-125">Accept</span></span>|<span data-ttu-id="95382-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95382-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95382-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="95382-127">Request body</span></span>
<span data-ttu-id="95382-128">Geben Sie im Textkörper Anforderung für das Objekt EnrollmentProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="95382-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="95382-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die EnrollmentProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="95382-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="95382-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="95382-130">Property</span></span>|<span data-ttu-id="95382-131">Typ</span><span class="sxs-lookup"><span data-stu-id="95382-131">Type</span></span>|<span data-ttu-id="95382-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95382-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95382-133">id</span><span class="sxs-lookup"><span data-stu-id="95382-133">id</span></span>|<span data-ttu-id="95382-134">String</span><span class="sxs-lookup"><span data-stu-id="95382-134">String</span></span>|<span data-ttu-id="95382-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="95382-135">The GUID for the object</span></span>|
|<span data-ttu-id="95382-136">displayName</span><span class="sxs-lookup"><span data-stu-id="95382-136">displayName</span></span>|<span data-ttu-id="95382-137">String</span><span class="sxs-lookup"><span data-stu-id="95382-137">String</span></span>|<span data-ttu-id="95382-138">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="95382-138">Name of the profile</span></span>|
|<span data-ttu-id="95382-139">description</span><span class="sxs-lookup"><span data-stu-id="95382-139">description</span></span>|<span data-ttu-id="95382-140">String</span><span class="sxs-lookup"><span data-stu-id="95382-140">String</span></span>|<span data-ttu-id="95382-141">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="95382-141">Description of the profile</span></span>|
|<span data-ttu-id="95382-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="95382-142">requiresUserAuthentication</span></span>|<span data-ttu-id="95382-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="95382-143">Boolean</span></span>|<span data-ttu-id="95382-144">Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert</span><span class="sxs-lookup"><span data-stu-id="95382-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="95382-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="95382-145">configurationEndpointUrl</span></span>|<span data-ttu-id="95382-146">String</span><span class="sxs-lookup"><span data-stu-id="95382-146">String</span></span>|<span data-ttu-id="95382-147">Endpunkt-Url für die Registrierung zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="95382-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="95382-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="95382-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="95382-149">Boolesch</span><span class="sxs-lookup"><span data-stu-id="95382-149">Boolean</span></span>|<span data-ttu-id="95382-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="95382-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="95382-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="95382-151">Response</span></span>
<span data-ttu-id="95382-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="95382-152">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95382-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="95382-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="95382-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="95382-154">Request</span></span>
<span data-ttu-id="95382-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="95382-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```

### <a name="response"></a><span data-ttu-id="95382-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="95382-156">Response</span></span>
<span data-ttu-id="95382-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="95382-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```





