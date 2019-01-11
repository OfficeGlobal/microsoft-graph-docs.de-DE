---
title: Liste depIOSEnrollmentProfiles
description: Listeneigenschaften und Beziehungen der DepIOSEnrollmentProfile-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ade3539e14d39ba6285662bfa7e876726252c5e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817178"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="632b2-103">Liste depIOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="632b2-103">List depIOSEnrollmentProfiles</span></span>

> <span data-ttu-id="632b2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="632b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="632b2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="632b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="632b2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="632b2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="632b2-107">Listeneigenschaften und Beziehungen der [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="632b2-107">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="632b2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="632b2-108">Prerequisites</span></span>
<span data-ttu-id="632b2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="632b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="632b2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="632b2-111">Permission type</span></span>|<span data-ttu-id="632b2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="632b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="632b2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="632b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="632b2-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="632b2-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="632b2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="632b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="632b2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="632b2-116">Not supported.</span></span>|
|<span data-ttu-id="632b2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="632b2-117">Application</span></span>|<span data-ttu-id="632b2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="632b2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="632b2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="632b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="632b2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="632b2-120">Request headers</span></span>
|<span data-ttu-id="632b2-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="632b2-121">Header</span></span>|<span data-ttu-id="632b2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="632b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="632b2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="632b2-123">Authorization</span></span>|<span data-ttu-id="632b2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="632b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="632b2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="632b2-125">Accept</span></span>|<span data-ttu-id="632b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="632b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="632b2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="632b2-127">Request body</span></span>
<span data-ttu-id="632b2-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="632b2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="632b2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="632b2-129">Response</span></span>
<span data-ttu-id="632b2-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="632b2-130">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="632b2-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="632b2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="632b2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="632b2-132">Request</span></span>
<span data-ttu-id="632b2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="632b2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="632b2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="632b2-134">Response</span></span>
<span data-ttu-id="632b2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="632b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1559

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
      "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
      "iTunesPairingMode": "allow",
      "managementCertificates": [
        {
          "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
          "thumbprint": "Thumbprint value",
          "certificate": "Certificate value"
        }
      ],
      "restoreFromAndroidDisabled": true,
      "awaitDeviceConfiguredConfirmation": true,
      "sharedIPadMaximumUserCount": 10,
      "enableSharedIPad": true,
      "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
      "enableSingleAppEnrollmentMode": true
    }
  ]
}
```





