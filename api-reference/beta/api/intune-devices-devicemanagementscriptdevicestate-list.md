---
title: Liste deviceManagementScriptDeviceStates
description: Listeneigenschaften und Beziehungen der DeviceManagementScriptDeviceState-Objekte.
ms.openlocfilehash: 1c419663960c14a834360839861c6adaff146935
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058789"
---
# <a name="list-devicemanagementscriptdevicestates"></a><span data-ttu-id="baaea-103">Liste deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="baaea-103">List deviceManagementScriptDeviceStates</span></span>

> <span data-ttu-id="baaea-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="baaea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="baaea-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="baaea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="baaea-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="baaea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="baaea-107">Listeneigenschaften und Beziehungen der [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="baaea-107">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="baaea-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="baaea-108">Prerequisites</span></span>
<span data-ttu-id="baaea-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baaea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baaea-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="baaea-111">Permission type</span></span>|<span data-ttu-id="baaea-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="baaea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baaea-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="baaea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="baaea-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="baaea-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="baaea-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="baaea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baaea-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="baaea-116">Not supported.</span></span>|
|<span data-ttu-id="baaea-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="baaea-117">Application</span></span>|<span data-ttu-id="baaea-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="baaea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="baaea-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="baaea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="baaea-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="baaea-120">Request headers</span></span>
|<span data-ttu-id="baaea-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="baaea-121">Header</span></span>|<span data-ttu-id="baaea-122">Wert</span><span class="sxs-lookup"><span data-stu-id="baaea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baaea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="baaea-123">Authorization</span></span>|<span data-ttu-id="baaea-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="baaea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baaea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="baaea-125">Accept</span></span>|<span data-ttu-id="baaea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="baaea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baaea-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="baaea-127">Request body</span></span>
<span data-ttu-id="baaea-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="baaea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baaea-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="baaea-129">Response</span></span>
<span data-ttu-id="baaea-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="baaea-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baaea-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="baaea-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="baaea-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="baaea-132">Request</span></span>
<span data-ttu-id="baaea-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="baaea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="baaea-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="baaea-134">Response</span></span>
<span data-ttu-id="baaea-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="baaea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
      "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
      "runState": "success",
      "resultMessage": "Result Message value",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "errorCode": 9,
      "errorDescription": "Error Description value"
    }
  ]
}
```





