---
title: EnrollmentProfile aktualisieren
description: Aktualisieren der Eigenschaften eines enrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 222d8fbe049e7a66ecc0094f179e1dae6b187054
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975042"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="18f06-103">EnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="18f06-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="18f06-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18f06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18f06-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="18f06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18f06-106">Aktualisieren der Eigenschaften eines [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="18f06-106">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18f06-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="18f06-107">Prerequisites</span></span>
<span data-ttu-id="18f06-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18f06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18f06-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18f06-110">Permission type</span></span>|<span data-ttu-id="18f06-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18f06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18f06-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18f06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18f06-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f06-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="18f06-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18f06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18f06-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18f06-115">Not supported.</span></span>|
|<span data-ttu-id="18f06-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18f06-116">Application</span></span>|<span data-ttu-id="18f06-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18f06-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18f06-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18f06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="18f06-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18f06-119">Request headers</span></span>
|<span data-ttu-id="18f06-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="18f06-120">Header</span></span>|<span data-ttu-id="18f06-121">Wert</span><span class="sxs-lookup"><span data-stu-id="18f06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18f06-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18f06-122">Authorization</span></span>|<span data-ttu-id="18f06-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="18f06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18f06-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="18f06-124">Accept</span></span>|<span data-ttu-id="18f06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18f06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18f06-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18f06-126">Request body</span></span>
<span data-ttu-id="18f06-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="18f06-127">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="18f06-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="18f06-128">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="18f06-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="18f06-129">Property</span></span>|<span data-ttu-id="18f06-130">Typ</span><span class="sxs-lookup"><span data-stu-id="18f06-130">Type</span></span>|<span data-ttu-id="18f06-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18f06-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18f06-132">id</span><span class="sxs-lookup"><span data-stu-id="18f06-132">id</span></span>|<span data-ttu-id="18f06-133">String</span><span class="sxs-lookup"><span data-stu-id="18f06-133">String</span></span>|<span data-ttu-id="18f06-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="18f06-134">The GUID for the object</span></span>|
|<span data-ttu-id="18f06-135">displayName</span><span class="sxs-lookup"><span data-stu-id="18f06-135">displayName</span></span>|<span data-ttu-id="18f06-136">String</span><span class="sxs-lookup"><span data-stu-id="18f06-136">String</span></span>|<span data-ttu-id="18f06-137">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="18f06-137">Name of the profile</span></span>|
|<span data-ttu-id="18f06-138">description</span><span class="sxs-lookup"><span data-stu-id="18f06-138">description</span></span>|<span data-ttu-id="18f06-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="18f06-139">String</span></span>|<span data-ttu-id="18f06-140">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="18f06-140">Description of the profile</span></span>|
|<span data-ttu-id="18f06-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="18f06-141">requiresUserAuthentication</span></span>|<span data-ttu-id="18f06-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="18f06-142">Boolean</span></span>|<span data-ttu-id="18f06-143">Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert.</span><span class="sxs-lookup"><span data-stu-id="18f06-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="18f06-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="18f06-144">configurationEndpointUrl</span></span>|<span data-ttu-id="18f06-145">String</span><span class="sxs-lookup"><span data-stu-id="18f06-145">String</span></span>|<span data-ttu-id="18f06-146">Konfigurations Endpunkt-URL für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="18f06-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="18f06-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="18f06-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="18f06-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="18f06-148">Boolean</span></span>|<span data-ttu-id="18f06-149">Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll.</span><span class="sxs-lookup"><span data-stu-id="18f06-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="18f06-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="18f06-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="18f06-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="18f06-151">Boolean</span></span>|<span data-ttu-id="18f06-152">Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten für registrierte Geräte erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="18f06-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="18f06-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="18f06-153">Response</span></span>
<span data-ttu-id="18f06-154">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="18f06-154">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18f06-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18f06-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="18f06-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18f06-156">Request</span></span>
<span data-ttu-id="18f06-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18f06-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18f06-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="18f06-158">Response</span></span>
<span data-ttu-id="18f06-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18f06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




