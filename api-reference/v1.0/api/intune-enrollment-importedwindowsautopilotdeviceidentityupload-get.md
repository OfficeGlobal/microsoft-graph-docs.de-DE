---
title: Abrufen von importedWindowsAutopilotDeviceIdentityUpload
description: Lesen Sie Eigenschaften und Beziehungen des ImportedWindowsAutopilotDeviceIdentityUpload-Objekts.
ms.openlocfilehash: 6d22366add6f6850fdd75d8ba8374584d5b5e558
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018709"
---
# <a name="get-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="d37c8-103">Abrufen von importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="d37c8-103">Get importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="d37c8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d37c8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d37c8-105">Lesen Sie Eigenschaften und Beziehungen des [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d37c8-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d37c8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d37c8-106">Prerequisites</span></span>
<span data-ttu-id="d37c8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d37c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d37c8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d37c8-109">Permission type</span></span>|<span data-ttu-id="d37c8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d37c8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d37c8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d37c8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d37c8-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d37c8-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d37c8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d37c8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d37c8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d37c8-114">Not supported.</span></span>|
|<span data-ttu-id="d37c8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d37c8-115">Application</span></span>|<span data-ttu-id="d37c8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d37c8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d37c8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d37c8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d37c8-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d37c8-118">Optional query parameters</span></span>
<span data-ttu-id="d37c8-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d37c8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d37c8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d37c8-120">Request headers</span></span>
|<span data-ttu-id="d37c8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d37c8-121">Header</span></span>|<span data-ttu-id="d37c8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d37c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d37c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d37c8-123">Authorization</span></span>|<span data-ttu-id="d37c8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d37c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d37c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d37c8-125">Accept</span></span>|<span data-ttu-id="d37c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d37c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d37c8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d37c8-127">Request body</span></span>
<span data-ttu-id="d37c8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d37c8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d37c8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d37c8-129">Response</span></span>
<span data-ttu-id="d37c8-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d37c8-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d37c8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d37c8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d37c8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d37c8-132">Request</span></span>
<span data-ttu-id="d37c8-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d37c8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

### <a name="response"></a><span data-ttu-id="d37c8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d37c8-134">Response</span></span>
<span data-ttu-id="d37c8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d37c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
    "id": "8d639524-9524-8d63-2495-638d2495638d",
    "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
    "status": "pending"
  }
}
```



