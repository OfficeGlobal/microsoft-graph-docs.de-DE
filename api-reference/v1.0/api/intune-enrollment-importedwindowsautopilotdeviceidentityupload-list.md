---
title: Liste importedWindowsAutopilotDeviceIdentityUploads
description: Listeneigenschaften und Beziehungen der ImportedWindowsAutopilotDeviceIdentityUpload-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6fad9ad4fca9dccd1b6aa402795248e5fc67734f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857316"
---
# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="fb801-103">Liste importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="fb801-103">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="fb801-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fb801-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb801-105">Listeneigenschaften und Beziehungen der [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="fb801-105">List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb801-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fb801-106">Prerequisites</span></span>
<span data-ttu-id="fb801-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb801-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb801-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fb801-109">Permission type</span></span>|<span data-ttu-id="fb801-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fb801-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb801-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fb801-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb801-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb801-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fb801-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fb801-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb801-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fb801-114">Not supported.</span></span>|
|<span data-ttu-id="fb801-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fb801-115">Application</span></span>|<span data-ttu-id="fb801-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fb801-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb801-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb801-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="fb801-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fb801-118">Request headers</span></span>
|<span data-ttu-id="fb801-119">Header</span><span class="sxs-lookup"><span data-stu-id="fb801-119">Header</span></span>|<span data-ttu-id="fb801-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fb801-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb801-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb801-121">Authorization</span></span>|<span data-ttu-id="fb801-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fb801-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb801-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fb801-123">Accept</span></span>|<span data-ttu-id="fb801-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fb801-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb801-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fb801-125">Request body</span></span>
<span data-ttu-id="fb801-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fb801-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb801-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb801-127">Response</span></span>
<span data-ttu-id="fb801-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="fb801-128">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb801-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fb801-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb801-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb801-130">Request</span></span>
<span data-ttu-id="fb801-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fb801-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="fb801-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb801-132">Response</span></span>
<span data-ttu-id="fb801-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fb801-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
      "id": "8d639524-9524-8d63-2495-638d2495638d",
      "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
      "status": "pending"
    }
  ]
}
```



