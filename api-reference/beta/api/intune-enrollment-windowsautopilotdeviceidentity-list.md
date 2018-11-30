---
title: Liste windowsAutopilotDeviceIdentities
description: Listeneigenschaften und Beziehungen der WindowsAutopilotDeviceIdentity-Objekte.
ms.openlocfilehash: 13ded8463d696b6eecdb11c84f9d40f1ba414e8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060087"
---
# <a name="list-windowsautopilotdeviceidentities"></a><span data-ttu-id="806ee-103">Liste windowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="806ee-103">List windowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="806ee-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="806ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="806ee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="806ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="806ee-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="806ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="806ee-107">Listeneigenschaften und Beziehungen der [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="806ee-107">List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="806ee-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="806ee-108">Prerequisites</span></span>
<span data-ttu-id="806ee-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="806ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="806ee-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="806ee-111">Permission type</span></span>|<span data-ttu-id="806ee-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="806ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="806ee-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="806ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="806ee-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="806ee-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="806ee-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="806ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="806ee-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="806ee-116">Not supported.</span></span>|
|<span data-ttu-id="806ee-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="806ee-117">Application</span></span>|<span data-ttu-id="806ee-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="806ee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="806ee-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="806ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="806ee-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="806ee-120">Request headers</span></span>
|<span data-ttu-id="806ee-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="806ee-121">Header</span></span>|<span data-ttu-id="806ee-122">Wert</span><span class="sxs-lookup"><span data-stu-id="806ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="806ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="806ee-123">Authorization</span></span>|<span data-ttu-id="806ee-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="806ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="806ee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="806ee-125">Accept</span></span>|<span data-ttu-id="806ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="806ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="806ee-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="806ee-127">Request body</span></span>
<span data-ttu-id="806ee-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="806ee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="806ee-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="806ee-129">Response</span></span>
<span data-ttu-id="806ee-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="806ee-130">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="806ee-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="806ee-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="806ee-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="806ee-132">Request</span></span>
<span data-ttu-id="806ee-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="806ee-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="806ee-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="806ee-134">Response</span></span>
<span data-ttu-id="806ee-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="806ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





