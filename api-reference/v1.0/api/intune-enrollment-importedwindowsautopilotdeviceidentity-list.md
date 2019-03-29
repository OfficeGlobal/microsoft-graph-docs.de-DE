---
title: importedWindowsAutopilotDeviceIdentities auflisten
description: Auflisten von Eigenschaften und Beziehungen der importedWindowsAutopilotDeviceIdentity-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e65a91af12b7f1689253ed95da341abd9d1aee36
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979347"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="7ada8-103">importedWindowsAutopilotDeviceIdentities auflisten</span><span class="sxs-lookup"><span data-stu-id="7ada8-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="7ada8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7ada8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ada8-105">Auflisten von Eigenschaften und Beziehungen der [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="7ada8-105">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ada8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7ada8-106">Prerequisites</span></span>
<span data-ttu-id="7ada8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ada8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ada8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ada8-109">Permission type</span></span>|<span data-ttu-id="7ada8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ada8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ada8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ada8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ada8-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ada8-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7ada8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ada8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ada8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ada8-114">Not supported.</span></span>|
|<span data-ttu-id="7ada8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ada8-115">Application</span></span>|<span data-ttu-id="7ada8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ada8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ada8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ada8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="7ada8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ada8-118">Request headers</span></span>
|<span data-ttu-id="7ada8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7ada8-119">Header</span></span>|<span data-ttu-id="7ada8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7ada8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ada8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ada8-121">Authorization</span></span>|<span data-ttu-id="7ada8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7ada8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ada8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7ada8-123">Accept</span></span>|<span data-ttu-id="7ada8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7ada8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ada8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ada8-125">Request body</span></span>
<span data-ttu-id="7ada8-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7ada8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ada8-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ada8-127">Response</span></span>
<span data-ttu-id="7ada8-128">Bei Erfolg gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) im Textkörper zurück.</span><span class="sxs-lookup"><span data-stu-id="7ada8-128">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ada8-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ada8-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ada8-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ada8-130">Request</span></span>
<span data-ttu-id="7ada8-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ada8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="7ada8-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ada8-132">Response</span></span>
<span data-ttu-id="7ada8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ada8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": [
    {
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
  ]
}
```



