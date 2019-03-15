---
title: ActiveDirectoryWindowsAutopilotDeploymentProfile abrufen
description: Lesen von Eigenschaften und Beziehungen des activeDirectoryWindowsAutopilotDeploymentProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01aec0eebc85fde7206b05be357010e96a41a5ea
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571977"
---
# <a name="get-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="a4b8a-103">ActiveDirectoryWindowsAutopilotDeploymentProfile abrufen</span><span class="sxs-lookup"><span data-stu-id="a4b8a-103">Get activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="a4b8a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a4b8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4b8a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a4b8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4b8a-106">Lesen von Eigenschaften und Beziehungen des [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a4b8a-106">Read properties and relationships of the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4b8a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a4b8a-107">Prerequisites</span></span>
<span data-ttu-id="a4b8a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a4b8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a4b8a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a4b8a-110">Permission type</span></span>|<span data-ttu-id="a4b8a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a4b8a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4b8a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a4b8a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4b8a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4b8a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a4b8a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a4b8a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4b8a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4b8a-115">Not supported.</span></span>|
|<span data-ttu-id="a4b8a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a4b8a-116">Application</span></span>|<span data-ttu-id="a4b8a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4b8a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4b8a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4b8a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4b8a-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a4b8a-119">Optional query parameters</span></span>
<span data-ttu-id="a4b8a-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a4b8a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4b8a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a4b8a-121">Request headers</span></span>
|<span data-ttu-id="a4b8a-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a4b8a-122">Header</span></span>|<span data-ttu-id="a4b8a-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a4b8a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4b8a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4b8a-124">Authorization</span></span>|<span data-ttu-id="a4b8a-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a4b8a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4b8a-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a4b8a-126">Accept</span></span>|<span data-ttu-id="a4b8a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a4b8a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4b8a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a4b8a-128">Request body</span></span>
<span data-ttu-id="a4b8a-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a4b8a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4b8a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4b8a-130">Response</span></span>
<span data-ttu-id="a4b8a-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a4b8a-131">If successful, this method returns a `200 OK` response code and [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4b8a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a4b8a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4b8a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4b8a-133">Request</span></span>
<span data-ttu-id="a4b8a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a4b8a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="a4b8a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4b8a-135">Response</span></span>
<span data-ttu-id="a4b8a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4b8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1356

{
  "value": {
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
}
```




