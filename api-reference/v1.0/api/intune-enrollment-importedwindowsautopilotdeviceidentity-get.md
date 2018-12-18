---
title: importedWindowsAutopilotDeviceIdentity abrufen
description: Lesen von Eigenschaften und Beziehungen des importedWindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
ms.openlocfilehash: 0f9d1c80fae8144dc37110345f9162e3c006f9fc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309359"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="fa165-103">importedWindowsAutopilotDeviceIdentity abrufen</span><span class="sxs-lookup"><span data-stu-id="fa165-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="fa165-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa165-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa165-105">Lesen von Eigenschaften und Beziehungen des [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa165-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa165-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa165-106">Prerequisites</span></span>
<span data-ttu-id="fa165-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa165-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa165-109">Permission type</span></span>|<span data-ttu-id="fa165-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa165-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa165-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa165-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa165-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa165-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fa165-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa165-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa165-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa165-114">Not supported.</span></span>|
|<span data-ttu-id="fa165-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa165-115">Application</span></span>|<span data-ttu-id="fa165-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa165-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa165-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa165-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa165-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fa165-118">Optional query parameters</span></span>
<span data-ttu-id="fa165-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fa165-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fa165-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa165-120">Request headers</span></span>
|<span data-ttu-id="fa165-121">Header</span><span class="sxs-lookup"><span data-stu-id="fa165-121">Header</span></span>|<span data-ttu-id="fa165-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fa165-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa165-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fa165-123">Authorization</span></span>|<span data-ttu-id="fa165-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa165-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa165-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa165-125">Accept</span></span>|<span data-ttu-id="fa165-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa165-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa165-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa165-127">Request body</span></span>
<span data-ttu-id="fa165-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fa165-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa165-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa165-129">Response</span></span>
<span data-ttu-id="fa165-130">Bei Erfolg gibt die Methode den Antwortcode `200 OK` und ein [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fa165-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa165-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa165-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa165-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa165-132">Request</span></span>
<span data-ttu-id="fa165-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa165-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="fa165-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa165-134">Response</span></span>
<span data-ttu-id="fa165-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa165-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 635

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
    "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
    "orderIdentifier": "Order Identifier value",
    "serialNumber": "Serial Number value",
    "productKey": "Product Key value",
    "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
    "state": {
      "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
      "deviceImportStatus": "pending",
      "deviceRegistrationId": "Device Registration Id value",
      "deviceErrorCode": 15,
      "deviceErrorName": "Device Error Name value"
    }
  }
}
```



