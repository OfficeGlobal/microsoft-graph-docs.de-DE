---
title: executeAction-Aktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc4916bcc7056ade0bf935e31fa935933541b480
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982084"
---
# <a name="executeaction-action"></a><span data-ttu-id="fe0cd-103">executeAction-Aktion</span><span class="sxs-lookup"><span data-stu-id="fe0cd-103">executeAction action</span></span>

> <span data-ttu-id="fe0cd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe0cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe0cd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fe0cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe0cd-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fe0cd-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe0cd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fe0cd-107">Prerequisites</span></span>
<span data-ttu-id="fe0cd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe0cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe0cd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe0cd-110">Permission type</span></span>|<span data-ttu-id="fe0cd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe0cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe0cd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe0cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe0cd-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="fe0cd-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="fe0cd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe0cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe0cd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe0cd-115">Not supported.</span></span>|
|<span data-ttu-id="fe0cd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe0cd-116">Application</span></span>|<span data-ttu-id="fe0cd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe0cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe0cd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe0cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/executeAction
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="fe0cd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe0cd-119">Request headers</span></span>
|<span data-ttu-id="fe0cd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fe0cd-120">Header</span></span>|<span data-ttu-id="fe0cd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fe0cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe0cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe0cd-122">Authorization</span></span>|<span data-ttu-id="fe0cd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fe0cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe0cd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fe0cd-124">Accept</span></span>|<span data-ttu-id="fe0cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe0cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe0cd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe0cd-126">Request body</span></span>
<span data-ttu-id="fe0cd-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="fe0cd-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fe0cd-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="fe0cd-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fe0cd-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fe0cd-129">Property</span></span>|<span data-ttu-id="fe0cd-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fe0cd-130">Type</span></span>|<span data-ttu-id="fe0cd-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe0cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe0cd-132">actionName</span><span class="sxs-lookup"><span data-stu-id="fe0cd-132">actionName</span></span>|[<span data-ttu-id="fe0cd-133">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="fe0cd-133">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="fe0cd-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="fe0cd-134">Not yet documented</span></span>|
|<span data-ttu-id="fe0cd-135">deviceIds</span><span class="sxs-lookup"><span data-stu-id="fe0cd-135">deviceIds</span></span>|<span data-ttu-id="fe0cd-136">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fe0cd-136">String collection</span></span>|<span data-ttu-id="fe0cd-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="fe0cd-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fe0cd-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe0cd-138">Response</span></span>
<span data-ttu-id="fe0cd-139">Bei erfolgreicher Ausführung gibt die Aktion den `200 OK` Antwortcode und eine [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fe0cd-139">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe0cd-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe0cd-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe0cd-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe0cd-141">Request</span></span>
<span data-ttu-id="fe0cd-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe0cd-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fe0cd-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe0cd-143">Response</span></span>
<span data-ttu-id="fe0cd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe0cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




