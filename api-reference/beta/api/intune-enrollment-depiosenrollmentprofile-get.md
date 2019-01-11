---
title: Abrufen von depIOSEnrollmentProfile
description: Lesen Sie Eigenschaften und Beziehungen des DepIOSEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4b1e2539e157d815f94a3eb3358665de70de80a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808106"
---
# <a name="get-depiosenrollmentprofile"></a><span data-ttu-id="ca2dc-103">Abrufen von depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ca2dc-103">Get depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="ca2dc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ca2dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca2dc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca2dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca2dc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ca2dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca2dc-107">Lesen Sie Eigenschaften und Beziehungen des [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ca2dc-107">Read properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca2dc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ca2dc-108">Prerequisites</span></span>
<span data-ttu-id="ca2dc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca2dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca2dc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ca2dc-111">Permission type</span></span>|<span data-ttu-id="ca2dc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ca2dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca2dc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ca2dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca2dc-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca2dc-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ca2dc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ca2dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca2dc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca2dc-116">Not supported.</span></span>|
|<span data-ttu-id="ca2dc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ca2dc-117">Application</span></span>|<span data-ttu-id="ca2dc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca2dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca2dc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca2dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca2dc-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ca2dc-120">Optional query parameters</span></span>
<span data-ttu-id="ca2dc-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ca2dc-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ca2dc-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ca2dc-122">Request headers</span></span>
|<span data-ttu-id="ca2dc-123">Header</span><span class="sxs-lookup"><span data-stu-id="ca2dc-123">Header</span></span>|<span data-ttu-id="ca2dc-124">Wert</span><span class="sxs-lookup"><span data-stu-id="ca2dc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca2dc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca2dc-125">Authorization</span></span>|<span data-ttu-id="ca2dc-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ca2dc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca2dc-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ca2dc-127">Accept</span></span>|<span data-ttu-id="ca2dc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ca2dc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca2dc-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ca2dc-129">Request body</span></span>
<span data-ttu-id="ca2dc-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ca2dc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca2dc-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca2dc-131">Response</span></span>
<span data-ttu-id="ca2dc-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DepIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ca2dc-132">If successful, this method returns a `200 OK` response code and [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca2dc-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ca2dc-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca2dc-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca2dc-134">Request</span></span>
<span data-ttu-id="ca2dc-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ca2dc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="ca2dc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca2dc-136">Response</span></span>
<span data-ttu-id="ca2dc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ca2dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1471

{
  "value": {
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
}
```





