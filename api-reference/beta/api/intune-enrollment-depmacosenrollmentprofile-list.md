---
title: Liste depMacOSEnrollmentProfiles
description: Listeneigenschaften und Beziehungen der DepMacOSEnrollmentProfile-Objekte.
author: tfitzmac
ms.openlocfilehash: 1c2b5ab4fbf333eb0bac6a57b9696e986e2c68fe
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321511"
---
# <a name="list-depmacosenrollmentprofiles"></a><span data-ttu-id="ea07d-103">Liste depMacOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="ea07d-103">List depMacOSEnrollmentProfiles</span></span>

> <span data-ttu-id="ea07d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ea07d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea07d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea07d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea07d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ea07d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea07d-107">Listeneigenschaften und Beziehungen der [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="ea07d-107">List properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea07d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea07d-108">Prerequisites</span></span>
<span data-ttu-id="ea07d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea07d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea07d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea07d-111">Permission type</span></span>|<span data-ttu-id="ea07d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea07d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea07d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea07d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea07d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea07d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ea07d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea07d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea07d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea07d-116">Not supported.</span></span>|
|<span data-ttu-id="ea07d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea07d-117">Application</span></span>|<span data-ttu-id="ea07d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea07d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea07d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea07d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ea07d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea07d-120">Request headers</span></span>
|<span data-ttu-id="ea07d-121">Header</span><span class="sxs-lookup"><span data-stu-id="ea07d-121">Header</span></span>|<span data-ttu-id="ea07d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ea07d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea07d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ea07d-123">Authorization</span></span>|<span data-ttu-id="ea07d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ea07d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea07d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea07d-125">Accept</span></span>|<span data-ttu-id="ea07d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea07d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea07d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea07d-127">Request body</span></span>
<span data-ttu-id="ea07d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ea07d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea07d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea07d-129">Response</span></span>
<span data-ttu-id="ea07d-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [DepMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ea07d-130">If successful, this method returns a `200 OK` response code and a collection of [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea07d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea07d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea07d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea07d-132">Request</span></span>
<span data-ttu-id="ea07d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea07d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="ea07d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea07d-134">Response</span></span>
<span data-ttu-id="ea07d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea07d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1114

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
      "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "isDefault": true,
      "supervisedModeEnabled": true,
      "supportDepartment": "Support Department value",
      "passCodeDisabled": true,
      "isMandatory": true,
      "locationDisabled": true,
      "supportPhoneNumber": "Support Phone Number value",
      "profileRemovalDisabled": true,
      "restoreBlocked": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "zoomDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true,
      "registrationDisabled": true,
      "fileVaultDisabled": true,
      "iCloudDiagnosticsDisabled": true
    }
  ]
}
```





