---
title: ActiveDirectoryWindowsAutopilotDeploymentProfiles aufListen
description: AufListen von Eigenschaften und Beziehungen der activeDirectoryWindowsAutopilotDeploymentProfile-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50e22ab4ce7218d21ce8a6f3c04ee2e715afeced
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571711"
---
# <a name="list-activedirectorywindowsautopilotdeploymentprofiles"></a><span data-ttu-id="dc670-103">ActiveDirectoryWindowsAutopilotDeploymentProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="dc670-103">List activeDirectoryWindowsAutopilotDeploymentProfiles</span></span>

> <span data-ttu-id="dc670-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dc670-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc670-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dc670-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc670-106">AufListen von Eigenschaften und Beziehungen der [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="dc670-106">List properties and relationships of the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc670-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dc670-107">Prerequisites</span></span>
<span data-ttu-id="dc670-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dc670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dc670-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dc670-110">Permission type</span></span>|<span data-ttu-id="dc670-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dc670-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc670-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dc670-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc670-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc670-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dc670-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dc670-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc670-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc670-115">Not supported.</span></span>|
|<span data-ttu-id="dc670-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dc670-116">Application</span></span>|<span data-ttu-id="dc670-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dc670-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc670-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc670-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="dc670-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dc670-119">Request headers</span></span>
|<span data-ttu-id="dc670-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dc670-120">Header</span></span>|<span data-ttu-id="dc670-121">Wert</span><span class="sxs-lookup"><span data-stu-id="dc670-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc670-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc670-122">Authorization</span></span>|<span data-ttu-id="dc670-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dc670-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc670-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dc670-124">Accept</span></span>|<span data-ttu-id="dc670-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc670-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc670-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dc670-126">Request body</span></span>
<span data-ttu-id="dc670-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dc670-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc670-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc670-128">Response</span></span>
<span data-ttu-id="dc670-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dc670-129">If successful, this method returns a `200 OK` response code and a collection of [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc670-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dc670-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc670-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dc670-131">Request</span></span>
<span data-ttu-id="dc670-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dc670-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
```

### <a name="response"></a><span data-ttu-id="dc670-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="dc670-133">Response</span></span>
<span data-ttu-id="dc670-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dc670-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1430

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
      "id": "49fe234a-234a-49fe-4a23-fe494a23fe49",
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
      "deviceType": "surfaceHub2",
      "enableWhiteGlove": true
    }
  ]
}
```




