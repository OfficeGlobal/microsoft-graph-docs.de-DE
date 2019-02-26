---
title: importedWindowsAutopilotDeviceIdentities auflisten
description: Auflisten von Eigenschaften und Beziehungen der importedWindowsAutopilotDeviceIdentity-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08dcbeac333b2d2364e73d54269780ab17c038c1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174172"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="240f1-103">importedWindowsAutopilotDeviceIdentities auflisten</span><span class="sxs-lookup"><span data-stu-id="240f1-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="240f1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="240f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="240f1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="240f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="240f1-106">Auflisten von Eigenschaften und Beziehungen der [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="240f1-106">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="240f1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="240f1-107">Prerequisites</span></span>
<span data-ttu-id="240f1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="240f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="240f1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="240f1-110">Permission type</span></span>|<span data-ttu-id="240f1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="240f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="240f1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="240f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="240f1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="240f1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="240f1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="240f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="240f1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="240f1-115">Not supported.</span></span>|
|<span data-ttu-id="240f1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="240f1-116">Application</span></span>|<span data-ttu-id="240f1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="240f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="240f1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="240f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="240f1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="240f1-119">Request headers</span></span>
|<span data-ttu-id="240f1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="240f1-120">Header</span></span>|<span data-ttu-id="240f1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="240f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="240f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="240f1-122">Authorization</span></span>|<span data-ttu-id="240f1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="240f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="240f1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="240f1-124">Accept</span></span>|<span data-ttu-id="240f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="240f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="240f1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="240f1-126">Request body</span></span>
<span data-ttu-id="240f1-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="240f1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="240f1-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="240f1-128">Response</span></span>
<span data-ttu-id="240f1-129">Bei Erfolg gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) im Textkörper zurück.</span><span class="sxs-lookup"><span data-stu-id="240f1-129">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="240f1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="240f1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="240f1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="240f1-131">Request</span></span>
<span data-ttu-id="240f1-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="240f1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="240f1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="240f1-133">Response</span></span>
<span data-ttu-id="240f1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="240f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




