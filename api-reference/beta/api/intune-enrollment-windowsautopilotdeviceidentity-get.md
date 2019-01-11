---
title: Abrufen von windowsAutopilotDeviceIdentity
description: Lesen Sie Eigenschaften und Beziehungen des WindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aba8b16b9704497f259fc1f931827f499bd3263c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873073"
---
# <a name="get-windowsautopilotdeviceidentity"></a><span data-ttu-id="fc45c-103">Abrufen von windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="fc45c-103">Get windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="fc45c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fc45c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc45c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc45c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc45c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fc45c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc45c-107">Lesen Sie Eigenschaften und Beziehungen des [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fc45c-107">Read properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc45c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fc45c-108">Prerequisites</span></span>
<span data-ttu-id="fc45c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc45c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc45c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc45c-111">Permission type</span></span>|<span data-ttu-id="fc45c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc45c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc45c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc45c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc45c-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc45c-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fc45c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc45c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc45c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc45c-116">Not supported.</span></span>|
|<span data-ttu-id="fc45c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc45c-117">Application</span></span>|<span data-ttu-id="fc45c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc45c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc45c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc45c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc45c-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fc45c-120">Optional query parameters</span></span>
<span data-ttu-id="fc45c-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fc45c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fc45c-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc45c-122">Request headers</span></span>
|<span data-ttu-id="fc45c-123">Header</span><span class="sxs-lookup"><span data-stu-id="fc45c-123">Header</span></span>|<span data-ttu-id="fc45c-124">Wert</span><span class="sxs-lookup"><span data-stu-id="fc45c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc45c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc45c-125">Authorization</span></span>|<span data-ttu-id="fc45c-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fc45c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc45c-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fc45c-127">Accept</span></span>|<span data-ttu-id="fc45c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fc45c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc45c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc45c-129">Request body</span></span>
<span data-ttu-id="fc45c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fc45c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc45c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc45c-131">Response</span></span>
<span data-ttu-id="fc45c-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fc45c-132">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc45c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc45c-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc45c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc45c-134">Request</span></span>
<span data-ttu-id="fc45c-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fc45c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="fc45c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc45c-136">Response</span></span>
<span data-ttu-id="fc45c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc45c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 853

{
  "value": {
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
}
```





