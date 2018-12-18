---
title: Liste azureADWindowsAutopilotDeploymentProfiles
description: Listeneigenschaften und Beziehungen der AzureADWindowsAutopilotDeploymentProfile-Objekte.
author: tfitzmac
ms.openlocfilehash: 0f68bf3856050fed0300498166eebc42a4cc13a5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356343"
---
# <a name="list-azureadwindowsautopilotdeploymentprofiles"></a><span data-ttu-id="77f9b-103">Liste azureADWindowsAutopilotDeploymentProfiles</span><span class="sxs-lookup"><span data-stu-id="77f9b-103">List azureADWindowsAutopilotDeploymentProfiles</span></span>

> <span data-ttu-id="77f9b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="77f9b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77f9b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77f9b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77f9b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="77f9b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77f9b-107">Listeneigenschaften und Beziehungen der [AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="77f9b-107">List properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77f9b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77f9b-108">Prerequisites</span></span>
<span data-ttu-id="77f9b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77f9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77f9b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77f9b-111">Permission type</span></span>|<span data-ttu-id="77f9b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77f9b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77f9b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77f9b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77f9b-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="77f9b-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="77f9b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77f9b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77f9b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77f9b-116">Not supported.</span></span>|
|<span data-ttu-id="77f9b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77f9b-117">Application</span></span>|<span data-ttu-id="77f9b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77f9b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77f9b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77f9b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="77f9b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77f9b-120">Request headers</span></span>
|<span data-ttu-id="77f9b-121">Header</span><span class="sxs-lookup"><span data-stu-id="77f9b-121">Header</span></span>|<span data-ttu-id="77f9b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="77f9b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77f9b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="77f9b-123">Authorization</span></span>|<span data-ttu-id="77f9b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77f9b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77f9b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77f9b-125">Accept</span></span>|<span data-ttu-id="77f9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77f9b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77f9b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77f9b-127">Request body</span></span>
<span data-ttu-id="77f9b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="77f9b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77f9b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="77f9b-129">Response</span></span>
<span data-ttu-id="77f9b-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="77f9b-130">If successful, this method returns a `200 OK` response code and a collection of [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77f9b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77f9b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="77f9b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77f9b-132">Request</span></span>
<span data-ttu-id="77f9b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77f9b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
```

### <a name="response"></a><span data-ttu-id="77f9b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="77f9b-134">Response</span></span>
<span data-ttu-id="77f9b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77f9b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1353

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
      "id": "e2ec4e69-4e69-e2ec-694e-ece2694eece2",
      "displayName": "Display Name value",
      "description": "Description value",
      "language": "Language value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "outOfBoxExperienceSettings": {
        "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
        "hidePrivacySettings": true,
        "hideEULA": true,
        "userType": "standard",
        "deviceUsageType": "shared",
        "skipKeyboardSelectionPage": true,
        "hideEscapeLink": true
      },
      "enrollmentStatusScreenSettings": {
        "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
        "hideInstallationProgress": true,
        "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
        "blockDeviceSetupRetryByUser": true,
        "allowLogCollectionOnInstallFailure": true,
        "customErrorMessage": "Custom Error Message value",
        "installProgressTimeoutInMinutes": 15,
        "allowDeviceUseOnInstallFailure": true
      },
      "extractHardwareHash": true,
      "deviceNameTemplate": "Device Name Template value"
    }
  ]
}
```





