---
title: EnrollmentProfile erstellen
description: Erstellen eines neuen enrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b38fe9bd6d418823cb2e94aa3fc8ac161ce471c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175115"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="61d10-103">EnrollmentProfile erstellen</span><span class="sxs-lookup"><span data-stu-id="61d10-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="61d10-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61d10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61d10-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="61d10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61d10-106">Erstellen eines neuen [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="61d10-106">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61d10-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="61d10-107">Prerequisites</span></span>
<span data-ttu-id="61d10-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="61d10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="61d10-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61d10-110">Permission type</span></span>|<span data-ttu-id="61d10-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61d10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61d10-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61d10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61d10-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61d10-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="61d10-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61d10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61d10-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61d10-115">Not supported.</span></span>|
|<span data-ttu-id="61d10-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61d10-116">Application</span></span>|<span data-ttu-id="61d10-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61d10-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61d10-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61d10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="61d10-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61d10-119">Request headers</span></span>
|<span data-ttu-id="61d10-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="61d10-120">Header</span></span>|<span data-ttu-id="61d10-121">Wert</span><span class="sxs-lookup"><span data-stu-id="61d10-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61d10-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61d10-122">Authorization</span></span>|<span data-ttu-id="61d10-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="61d10-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61d10-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="61d10-124">Accept</span></span>|<span data-ttu-id="61d10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61d10-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61d10-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61d10-126">Request body</span></span>
<span data-ttu-id="61d10-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das enrollmentProfile-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="61d10-127">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="61d10-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der enrollmentProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="61d10-128">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="61d10-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61d10-129">Property</span></span>|<span data-ttu-id="61d10-130">Typ</span><span class="sxs-lookup"><span data-stu-id="61d10-130">Type</span></span>|<span data-ttu-id="61d10-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61d10-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d10-132">id</span><span class="sxs-lookup"><span data-stu-id="61d10-132">id</span></span>|<span data-ttu-id="61d10-133">String</span><span class="sxs-lookup"><span data-stu-id="61d10-133">String</span></span>|<span data-ttu-id="61d10-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="61d10-134">The GUID for the object</span></span>|
|<span data-ttu-id="61d10-135">displayName</span><span class="sxs-lookup"><span data-stu-id="61d10-135">displayName</span></span>|<span data-ttu-id="61d10-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61d10-136">String</span></span>|<span data-ttu-id="61d10-137">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="61d10-137">Name of the profile</span></span>|
|<span data-ttu-id="61d10-138">description</span><span class="sxs-lookup"><span data-stu-id="61d10-138">description</span></span>|<span data-ttu-id="61d10-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61d10-139">String</span></span>|<span data-ttu-id="61d10-140">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="61d10-140">Description of the profile</span></span>|
|<span data-ttu-id="61d10-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="61d10-141">requiresUserAuthentication</span></span>|<span data-ttu-id="61d10-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="61d10-142">Boolean</span></span>|<span data-ttu-id="61d10-143">Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert.</span><span class="sxs-lookup"><span data-stu-id="61d10-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="61d10-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="61d10-144">configurationEndpointUrl</span></span>|<span data-ttu-id="61d10-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61d10-145">String</span></span>|<span data-ttu-id="61d10-146">Konfigurations Endpunkt-URL für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="61d10-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="61d10-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="61d10-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="61d10-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="61d10-148">Boolean</span></span>|<span data-ttu-id="61d10-149">Gibt an, dass der Apple-Setup-Assistent anstelle des Unternehmensportals authentifiziert werden soll.</span><span class="sxs-lookup"><span data-stu-id="61d10-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="61d10-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="61d10-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="61d10-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="61d10-151">Boolean</span></span>|<span data-ttu-id="61d10-152">Gibt an, dass das Unternehmens Portal auf dem Setup-Assistenten für registrierte Geräte erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="61d10-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="61d10-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="61d10-153">Response</span></span>
<span data-ttu-id="61d10-154">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="61d10-154">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61d10-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61d10-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="61d10-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61d10-156">Request</span></span>
<span data-ttu-id="61d10-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61d10-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="61d10-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="61d10-158">Response</span></span>
<span data-ttu-id="61d10-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61d10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




