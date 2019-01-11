---
title: EnrollmentProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines EnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9a5628ad6aff7926d4248e76e5203a9419fc1727
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822596"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="3af11-103">EnrollmentProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3af11-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="3af11-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3af11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3af11-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3af11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3af11-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3af11-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3af11-107">Aktualisieren Sie die Eigenschaften eines [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3af11-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3af11-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3af11-108">Prerequisites</span></span>
<span data-ttu-id="3af11-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3af11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3af11-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3af11-111">Permission type</span></span>|<span data-ttu-id="3af11-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3af11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3af11-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3af11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3af11-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3af11-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3af11-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3af11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3af11-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3af11-116">Not supported.</span></span>|
|<span data-ttu-id="3af11-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3af11-117">Application</span></span>|<span data-ttu-id="3af11-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3af11-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3af11-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3af11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="3af11-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3af11-120">Request headers</span></span>
|<span data-ttu-id="3af11-121">Header</span><span class="sxs-lookup"><span data-stu-id="3af11-121">Header</span></span>|<span data-ttu-id="3af11-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3af11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3af11-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3af11-123">Authorization</span></span>|<span data-ttu-id="3af11-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3af11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3af11-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3af11-125">Accept</span></span>|<span data-ttu-id="3af11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3af11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3af11-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3af11-127">Request body</span></span>
<span data-ttu-id="3af11-128">Geben Sie im Textkörper Anforderung für das Objekt [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="3af11-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="3af11-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="3af11-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="3af11-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3af11-130">Property</span></span>|<span data-ttu-id="3af11-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3af11-131">Type</span></span>|<span data-ttu-id="3af11-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3af11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3af11-133">id</span><span class="sxs-lookup"><span data-stu-id="3af11-133">id</span></span>|<span data-ttu-id="3af11-134">String</span><span class="sxs-lookup"><span data-stu-id="3af11-134">String</span></span>|<span data-ttu-id="3af11-135">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="3af11-135">The GUID for the object</span></span>|
|<span data-ttu-id="3af11-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3af11-136">displayName</span></span>|<span data-ttu-id="3af11-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3af11-137">String</span></span>|<span data-ttu-id="3af11-138">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="3af11-138">Name of the profile</span></span>|
|<span data-ttu-id="3af11-139">description</span><span class="sxs-lookup"><span data-stu-id="3af11-139">description</span></span>|<span data-ttu-id="3af11-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3af11-140">String</span></span>|<span data-ttu-id="3af11-141">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="3af11-141">Description of the profile</span></span>|
|<span data-ttu-id="3af11-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="3af11-142">requiresUserAuthentication</span></span>|<span data-ttu-id="3af11-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3af11-143">Boolean</span></span>|<span data-ttu-id="3af11-144">Gibt an, ob das Profil eine Benutzerauthentifizierung erfordert</span><span class="sxs-lookup"><span data-stu-id="3af11-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="3af11-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="3af11-145">configurationEndpointUrl</span></span>|<span data-ttu-id="3af11-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3af11-146">String</span></span>|<span data-ttu-id="3af11-147">Endpunkt-Url für die Registrierung zu verwendende Konfiguration</span><span class="sxs-lookup"><span data-stu-id="3af11-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="3af11-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="3af11-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="3af11-149">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3af11-149">Boolean</span></span>|<span data-ttu-id="3af11-150">Gibt an, dass die Authentifizierung mit Apple Setup-Assistenten anstelle von Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="3af11-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="3af11-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="3af11-151">Response</span></span>
<span data-ttu-id="3af11-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3af11-152">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3af11-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3af11-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="3af11-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3af11-154">Request</span></span>
<span data-ttu-id="3af11-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3af11-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 250

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```

### <a name="response"></a><span data-ttu-id="3af11-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="3af11-156">Response</span></span>
<span data-ttu-id="3af11-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3af11-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





