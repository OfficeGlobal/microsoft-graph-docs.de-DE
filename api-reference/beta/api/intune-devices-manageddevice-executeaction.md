---
title: ExecuteAction-Aktion
description: Noch nicht dokumentiert
ms.openlocfilehash: 1358b95bbb61aaef71df44c87ab6aeb0bc210761
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065318"
---
# <a name="executeaction-action"></a><span data-ttu-id="cf03d-103">ExecuteAction-Aktion</span><span class="sxs-lookup"><span data-stu-id="cf03d-103">executeAction action</span></span>

> <span data-ttu-id="cf03d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cf03d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf03d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cf03d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf03d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cf03d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf03d-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="cf03d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf03d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf03d-108">Prerequisites</span></span>
<span data-ttu-id="cf03d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf03d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf03d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf03d-111">Permission type</span></span>|<span data-ttu-id="cf03d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf03d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf03d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf03d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf03d-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="cf03d-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="cf03d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf03d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf03d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf03d-116">Not supported.</span></span>|
|<span data-ttu-id="cf03d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf03d-117">Application</span></span>|<span data-ttu-id="cf03d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf03d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf03d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf03d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/executeAction
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="cf03d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf03d-120">Request headers</span></span>
|<span data-ttu-id="cf03d-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cf03d-121">Header</span></span>|<span data-ttu-id="cf03d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cf03d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf03d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf03d-123">Authorization</span></span>|<span data-ttu-id="cf03d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf03d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf03d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf03d-125">Accept</span></span>|<span data-ttu-id="cf03d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf03d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf03d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf03d-127">Request body</span></span>
<span data-ttu-id="cf03d-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="cf03d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cf03d-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="cf03d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cf03d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cf03d-130">Property</span></span>|<span data-ttu-id="cf03d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="cf03d-131">Type</span></span>|<span data-ttu-id="cf03d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf03d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf03d-133">actionName</span><span class="sxs-lookup"><span data-stu-id="cf03d-133">actionName</span></span>|[<span data-ttu-id="cf03d-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="cf03d-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="cf03d-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="cf03d-135">Not yet documented</span></span>|
|<span data-ttu-id="cf03d-136">deviceIds</span><span class="sxs-lookup"><span data-stu-id="cf03d-136">deviceIds</span></span>|<span data-ttu-id="cf03d-137">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="cf03d-137">String collection</span></span>|<span data-ttu-id="cf03d-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="cf03d-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cf03d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf03d-139">Response</span></span>
<span data-ttu-id="cf03d-140">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [BulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cf03d-140">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf03d-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf03d-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf03d-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf03d-142">Request</span></span>
<span data-ttu-id="cf03d-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf03d-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/executeAction

Content-type: application/json
Content-length: 78

{
  "actionName": "delete",
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="cf03d-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf03d-144">Response</span></span>
<span data-ttu-id="cf03d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf03d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult",
    "successfulDeviceIds": [
      "Successful Device Ids value"
    ],
    "failedDeviceIds": [
      "Failed Device Ids value"
    ],
    "notFoundDeviceIds": [
      "Not Found Device Ids value"
    ],
    "notSupportedDeviceIds": [
      "Not Supported Device Ids value"
    ]
  }
}
```





