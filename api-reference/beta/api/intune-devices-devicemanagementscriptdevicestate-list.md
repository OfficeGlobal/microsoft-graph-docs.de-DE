---
title: DeviceManagementScriptDeviceStates aufListen
description: AufListen von Eigenschaften und Beziehungen der deviceManagementScriptDeviceState-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35f649d022694b7943153fd592aba2b3694b73d2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973593"
---
# <a name="list-devicemanagementscriptdevicestates"></a><span data-ttu-id="d1e58-103">DeviceManagementScriptDeviceStates aufListen</span><span class="sxs-lookup"><span data-stu-id="d1e58-103">List deviceManagementScriptDeviceStates</span></span>

> <span data-ttu-id="d1e58-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1e58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1e58-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d1e58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1e58-106">AufListen von Eigenschaften und Beziehungen der [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="d1e58-106">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1e58-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d1e58-107">Prerequisites</span></span>
<span data-ttu-id="d1e58-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1e58-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d1e58-110">Permission type</span></span>|<span data-ttu-id="d1e58-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d1e58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1e58-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d1e58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1e58-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1e58-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d1e58-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d1e58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1e58-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d1e58-115">Not supported.</span></span>|
|<span data-ttu-id="d1e58-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d1e58-116">Application</span></span>|<span data-ttu-id="d1e58-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d1e58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1e58-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1e58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="d1e58-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d1e58-119">Request headers</span></span>
|<span data-ttu-id="d1e58-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d1e58-120">Header</span></span>|<span data-ttu-id="d1e58-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d1e58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1e58-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1e58-122">Authorization</span></span>|<span data-ttu-id="d1e58-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d1e58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1e58-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d1e58-124">Accept</span></span>|<span data-ttu-id="d1e58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1e58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1e58-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d1e58-126">Request body</span></span>
<span data-ttu-id="d1e58-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d1e58-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1e58-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1e58-128">Response</span></span>
<span data-ttu-id="d1e58-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d1e58-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1e58-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d1e58-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1e58-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1e58-131">Request</span></span>
<span data-ttu-id="d1e58-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d1e58-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="d1e58-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1e58-133">Response</span></span>
<span data-ttu-id="d1e58-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1e58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




