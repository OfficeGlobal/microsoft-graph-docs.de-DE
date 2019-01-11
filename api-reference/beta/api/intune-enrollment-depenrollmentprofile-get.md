---
title: Abrufen von depEnrollmentProfile
description: Lesen Sie Eigenschaften und Beziehungen des DepEnrollmentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aa3c9da25c4afa0b8ba4130f6cc7afb869aa33f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878967"
---
# <a name="get-depenrollmentprofile"></a><span data-ttu-id="fc451-103">Abrufen von depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="fc451-103">Get depEnrollmentProfile</span></span>

> <span data-ttu-id="fc451-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fc451-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc451-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc451-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc451-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fc451-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc451-107">Lesen Sie Eigenschaften und Beziehungen des [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fc451-107">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc451-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fc451-108">Prerequisites</span></span>
<span data-ttu-id="fc451-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc451-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc451-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc451-111">Permission type</span></span>|<span data-ttu-id="fc451-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc451-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc451-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc451-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc451-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc451-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fc451-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc451-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc451-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc451-116">Not supported.</span></span>|
|<span data-ttu-id="fc451-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc451-117">Application</span></span>|<span data-ttu-id="fc451-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc451-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc451-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc451-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc451-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fc451-120">Optional query parameters</span></span>
<span data-ttu-id="fc451-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fc451-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fc451-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc451-122">Request headers</span></span>
|<span data-ttu-id="fc451-123">Header</span><span class="sxs-lookup"><span data-stu-id="fc451-123">Header</span></span>|<span data-ttu-id="fc451-124">Wert</span><span class="sxs-lookup"><span data-stu-id="fc451-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc451-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc451-125">Authorization</span></span>|<span data-ttu-id="fc451-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fc451-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc451-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fc451-127">Accept</span></span>|<span data-ttu-id="fc451-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fc451-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc451-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc451-129">Request body</span></span>
<span data-ttu-id="fc451-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fc451-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc451-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc451-131">Response</span></span>
<span data-ttu-id="fc451-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DepEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fc451-132">If successful, this method returns a `200 OK` response code and [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc451-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc451-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc451-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc451-134">Request</span></span>
<span data-ttu-id="fc451-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fc451-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="fc451-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc451-136">Response</span></span>
<span data-ttu-id="fc451-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc451-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1432

{
  "value": {
    "@odata.type": "#microsoft.graph.depEnrollmentProfile",
    "id": "3d4534f7-34f7-3d45-f734-453df734453d",
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
    "iTunesPairingMode": "allow",
    "profileRemovalDisabled": true,
    "managementCertificates": [
      {
        "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
        "thumbprint": "Thumbprint value",
        "certificate": "Certificate value"
      }
    ],
    "restoreBlocked": true,
    "restoreFromAndroidDisabled": true,
    "appleIdDisabled": true,
    "termsAndConditionsDisabled": true,
    "touchIdDisabled": true,
    "applePayDisabled": true,
    "zoomDisabled": true,
    "siriDisabled": true,
    "diagnosticsDisabled": true,
    "macOSRegistrationDisabled": true,
    "macOSFileVaultDisabled": true,
    "awaitDeviceConfiguredConfirmation": true,
    "sharedIPadMaximumUserCount": 10,
    "enableSharedIPad": true
  }
}
```





