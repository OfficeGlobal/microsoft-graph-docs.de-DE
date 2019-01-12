---
title: importedWindowsAutopilotDeviceIdentity abrufen
description: Lesen von Eigenschaften und Beziehungen des importedWindowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e46771b73082ac8b1f3b70a6a694f3392417bc5b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943515"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="88c97-103">importedWindowsAutopilotDeviceIdentity abrufen</span><span class="sxs-lookup"><span data-stu-id="88c97-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="88c97-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="88c97-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88c97-105">Lesen von Eigenschaften und Beziehungen des [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="88c97-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88c97-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="88c97-106">Prerequisites</span></span>
<span data-ttu-id="88c97-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88c97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88c97-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="88c97-109">Permission type</span></span>|<span data-ttu-id="88c97-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="88c97-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88c97-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="88c97-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88c97-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c97-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="88c97-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="88c97-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88c97-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88c97-114">Not supported.</span></span>|
|<span data-ttu-id="88c97-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="88c97-115">Application</span></span>|<span data-ttu-id="88c97-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88c97-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88c97-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="88c97-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88c97-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="88c97-118">Optional query parameters</span></span>
<span data-ttu-id="88c97-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="88c97-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="88c97-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="88c97-120">Request headers</span></span>
|<span data-ttu-id="88c97-121">Header</span><span class="sxs-lookup"><span data-stu-id="88c97-121">Header</span></span>|<span data-ttu-id="88c97-122">Wert</span><span class="sxs-lookup"><span data-stu-id="88c97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88c97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88c97-123">Authorization</span></span>|<span data-ttu-id="88c97-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="88c97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88c97-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="88c97-125">Accept</span></span>|<span data-ttu-id="88c97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88c97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88c97-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="88c97-127">Request body</span></span>
<span data-ttu-id="88c97-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="88c97-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88c97-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="88c97-129">Response</span></span>
<span data-ttu-id="88c97-130">Bei Erfolg gibt die Methode den Antwortcode `200 OK` und ein [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="88c97-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88c97-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="88c97-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="88c97-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="88c97-132">Request</span></span>
<span data-ttu-id="88c97-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="88c97-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="88c97-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="88c97-134">Response</span></span>
<span data-ttu-id="88c97-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="88c97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



