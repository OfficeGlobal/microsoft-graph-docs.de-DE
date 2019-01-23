---
title: Liste activeDirectoryWindowsAutopilotDeploymentProfiles
description: Listeneigenschaften und Beziehungen der ActiveDirectoryWindowsAutopilotDeploymentProfile-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 37e05d2a8a6a33f90b80aaf82a23badb6171e939
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411533"
---
# <a name="list-activedirectorywindowsautopilotdeploymentprofiles"></a><span data-ttu-id="ccd17-103">Liste activeDirectoryWindowsAutopilotDeploymentProfiles</span><span class="sxs-lookup"><span data-stu-id="ccd17-103">List activeDirectoryWindowsAutopilotDeploymentProfiles</span></span>

> <span data-ttu-id="ccd17-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ccd17-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ccd17-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ccd17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccd17-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ccd17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccd17-107">Listeneigenschaften und Beziehungen der [ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="ccd17-107">List properties and relationships of the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccd17-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ccd17-108">Prerequisites</span></span>
<span data-ttu-id="ccd17-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ccd17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ccd17-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ccd17-111">Permission type</span></span>|<span data-ttu-id="ccd17-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ccd17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccd17-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ccd17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccd17-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd17-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ccd17-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ccd17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccd17-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ccd17-116">Not supported.</span></span>|
|<span data-ttu-id="ccd17-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ccd17-117">Application</span></span>|<span data-ttu-id="ccd17-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ccd17-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccd17-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ccd17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ccd17-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ccd17-120">Request headers</span></span>
|<span data-ttu-id="ccd17-121">Header</span><span class="sxs-lookup"><span data-stu-id="ccd17-121">Header</span></span>|<span data-ttu-id="ccd17-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ccd17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccd17-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ccd17-123">Authorization</span></span>|<span data-ttu-id="ccd17-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ccd17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccd17-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ccd17-125">Accept</span></span>|<span data-ttu-id="ccd17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ccd17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd17-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ccd17-127">Request body</span></span>
<span data-ttu-id="ccd17-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ccd17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccd17-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ccd17-129">Response</span></span>
<span data-ttu-id="ccd17-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [ActiveDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ccd17-130">If successful, this method returns a `200 OK` response code and a collection of [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccd17-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ccd17-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccd17-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ccd17-132">Request</span></span>
<span data-ttu-id="ccd17-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ccd17-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
```

### <a name="response"></a><span data-ttu-id="ccd17-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ccd17-134">Response</span></span>
<span data-ttu-id="ccd17-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ccd17-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

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
      "deviceNameTemplate": "Device Name Template value"
    }
  ]
}
```




