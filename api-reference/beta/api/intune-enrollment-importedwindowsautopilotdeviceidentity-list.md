---
title: importedWindowsAutopilotDeviceIdentities auflisten
description: Auflisten von Eigenschaften und Beziehungen der importedWindowsAutopilotDeviceIdentity-Objekte.
ms.openlocfilehash: 1ebaabefaa6fb49a9d1f12c6d6b1f7cb73818324
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063799"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="83f54-103">importedWindowsAutopilotDeviceIdentities auflisten</span><span class="sxs-lookup"><span data-stu-id="83f54-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="83f54-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="83f54-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83f54-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83f54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83f54-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="83f54-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83f54-107">Auflisten von Eigenschaften und Beziehungen der [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="83f54-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83f54-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="83f54-108">Prerequisites</span></span>
<span data-ttu-id="83f54-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83f54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83f54-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83f54-111">Permission type</span></span>|<span data-ttu-id="83f54-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83f54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83f54-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83f54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83f54-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83f54-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="83f54-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="83f54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83f54-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83f54-116">Not supported.</span></span>|
|<span data-ttu-id="83f54-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83f54-117">Application</span></span>|<span data-ttu-id="83f54-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83f54-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83f54-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83f54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="83f54-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83f54-120">Request headers</span></span>
|<span data-ttu-id="83f54-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="83f54-121">Header</span></span>|<span data-ttu-id="83f54-122">Wert</span><span class="sxs-lookup"><span data-stu-id="83f54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83f54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83f54-123">Authorization</span></span>|<span data-ttu-id="83f54-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="83f54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83f54-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83f54-125">Accept</span></span>|<span data-ttu-id="83f54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83f54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83f54-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83f54-127">Request body</span></span>
<span data-ttu-id="83f54-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="83f54-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83f54-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="83f54-129">Response</span></span>
<span data-ttu-id="83f54-130">Bei Erfolg gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) im Textkörper zurück.</span><span class="sxs-lookup"><span data-stu-id="83f54-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83f54-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="83f54-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="83f54-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83f54-132">Request</span></span>
<span data-ttu-id="83f54-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83f54-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="83f54-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="83f54-134">Response</span></span>
<span data-ttu-id="83f54-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="83f54-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




