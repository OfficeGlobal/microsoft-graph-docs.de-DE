---
title: WindowsAutopilotDeviceIdentities aufListen
description: AufListen von Eigenschaften und Beziehungen der windowsAutopilotDeviceIdentity-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33b44dbd8ed301db3343e9d01dd37fe47b2c04e8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148937"
---
# <a name="list-windowsautopilotdeviceidentities"></a><span data-ttu-id="53d75-103">WindowsAutopilotDeviceIdentities aufListen</span><span class="sxs-lookup"><span data-stu-id="53d75-103">List windowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="53d75-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53d75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53d75-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="53d75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53d75-106">AufListen von Eigenschaften und Beziehungen der [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="53d75-106">List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53d75-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53d75-107">Prerequisites</span></span>
<span data-ttu-id="53d75-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="53d75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="53d75-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53d75-110">Permission type</span></span>|<span data-ttu-id="53d75-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53d75-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53d75-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53d75-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53d75-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="53d75-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="53d75-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53d75-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53d75-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53d75-115">Not supported.</span></span>|
|<span data-ttu-id="53d75-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53d75-116">Application</span></span>|<span data-ttu-id="53d75-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53d75-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53d75-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53d75-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="53d75-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53d75-119">Request headers</span></span>
|<span data-ttu-id="53d75-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="53d75-120">Header</span></span>|<span data-ttu-id="53d75-121">Wert</span><span class="sxs-lookup"><span data-stu-id="53d75-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53d75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53d75-122">Authorization</span></span>|<span data-ttu-id="53d75-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="53d75-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53d75-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="53d75-124">Accept</span></span>|<span data-ttu-id="53d75-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53d75-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53d75-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53d75-126">Request body</span></span>
<span data-ttu-id="53d75-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="53d75-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53d75-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="53d75-128">Response</span></span>
<span data-ttu-id="53d75-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="53d75-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53d75-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53d75-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="53d75-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53d75-131">Request</span></span>
<span data-ttu-id="53d75-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53d75-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="53d75-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="53d75-133">Response</span></span>
<span data-ttu-id="53d75-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53d75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 897

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
      "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
      "deploymentProfileAssignmentStatus": "assignedInSync",
      "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
      "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
      "orderIdentifier": "Order Identifier value",
      "purchaseOrderIdentifier": "Purchase Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "enrollmentState": "enrolled",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "addressableUserName": "Addressable User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




