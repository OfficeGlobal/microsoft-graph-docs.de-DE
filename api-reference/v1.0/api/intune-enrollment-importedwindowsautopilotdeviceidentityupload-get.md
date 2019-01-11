---
title: Abrufen von importedWindowsAutopilotDeviceIdentityUpload
description: Lesen Sie Eigenschaften und Beziehungen des ImportedWindowsAutopilotDeviceIdentityUpload-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 369a1dadd706efc05db6029ab912e964f98bc620
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837037"
---
# <a name="get-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="4a4de-103">Abrufen von importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="4a4de-103">Get importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="4a4de-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4a4de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a4de-105">Lesen Sie Eigenschaften und Beziehungen des [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4a4de-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a4de-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4a4de-106">Prerequisites</span></span>
<span data-ttu-id="4a4de-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a4de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a4de-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a4de-109">Permission type</span></span>|<span data-ttu-id="4a4de-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a4de-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a4de-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a4de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4a4de-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a4de-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4a4de-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a4de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a4de-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a4de-114">Not supported.</span></span>|
|<span data-ttu-id="4a4de-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a4de-115">Application</span></span>|<span data-ttu-id="4a4de-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a4de-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a4de-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a4de-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a4de-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4a4de-118">Optional query parameters</span></span>
<span data-ttu-id="4a4de-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a4de-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4a4de-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a4de-120">Request headers</span></span>
|<span data-ttu-id="4a4de-121">Header</span><span class="sxs-lookup"><span data-stu-id="4a4de-121">Header</span></span>|<span data-ttu-id="4a4de-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4a4de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a4de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a4de-123">Authorization</span></span>|<span data-ttu-id="4a4de-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4a4de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a4de-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4a4de-125">Accept</span></span>|<span data-ttu-id="4a4de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a4de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a4de-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a4de-127">Request body</span></span>
<span data-ttu-id="4a4de-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4a4de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a4de-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a4de-129">Response</span></span>
<span data-ttu-id="4a4de-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4a4de-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a4de-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a4de-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a4de-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a4de-132">Request</span></span>
<span data-ttu-id="4a4de-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a4de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

### <a name="response"></a><span data-ttu-id="4a4de-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a4de-134">Response</span></span>
<span data-ttu-id="4a4de-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a4de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



