---
title: AzureADWindowsAutopilotDeploymentProfiles aufListen
description: AufListen von Eigenschaften und Beziehungen der azureADWindowsAutopilotDeploymentProfile-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6580b07a3a8d69dbbaa3a211d4b66638e9d66742
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165401"
---
# <a name="list-azureadwindowsautopilotdeploymentprofiles"></a><span data-ttu-id="df960-103">AzureADWindowsAutopilotDeploymentProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="df960-103">List azureADWindowsAutopilotDeploymentProfiles</span></span>

> <span data-ttu-id="df960-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df960-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df960-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="df960-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df960-106">AufListen von Eigenschaften und Beziehungen der [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="df960-106">List properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df960-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="df960-107">Prerequisites</span></span>
<span data-ttu-id="df960-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="df960-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="df960-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df960-110">Permission type</span></span>|<span data-ttu-id="df960-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df960-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df960-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df960-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df960-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="df960-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="df960-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df960-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df960-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df960-115">Not supported.</span></span>|
|<span data-ttu-id="df960-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df960-116">Application</span></span>|<span data-ttu-id="df960-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df960-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df960-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df960-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="df960-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="df960-119">Request headers</span></span>
|<span data-ttu-id="df960-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="df960-120">Header</span></span>|<span data-ttu-id="df960-121">Wert</span><span class="sxs-lookup"><span data-stu-id="df960-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df960-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df960-122">Authorization</span></span>|<span data-ttu-id="df960-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="df960-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df960-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="df960-124">Accept</span></span>|<span data-ttu-id="df960-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df960-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df960-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df960-126">Request body</span></span>
<span data-ttu-id="df960-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="df960-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df960-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="df960-128">Response</span></span>
<span data-ttu-id="df960-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="df960-129">If successful, this method returns a `200 OK` response code and a collection of [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df960-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df960-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="df960-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="df960-131">Request</span></span>
<span data-ttu-id="df960-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="df960-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
```

### <a name="response"></a><span data-ttu-id="df960-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="df960-133">Response</span></span>
<span data-ttu-id="df960-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df960-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1386

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
      "deviceNameTemplate": "Device Name Template value",
      "enableWhiteGlove": true
    }
  ]
}
```




