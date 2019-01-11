---
title: Abrufen von deviceManagementScriptDeviceState
description: Lesen Sie Eigenschaften und Beziehungen des DeviceManagementScriptDeviceState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fb82aec0d1e1a93f66986a8c2673ad92b7791d01
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849441"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="a2c0b-103">Abrufen von deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="a2c0b-103">Get deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="a2c0b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2c0b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2c0b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2c0b-107">Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-107">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2c0b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a2c0b-108">Prerequisites</span></span>
<span data-ttu-id="a2c0b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2c0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2c0b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2c0b-111">Permission type</span></span>|<span data-ttu-id="a2c0b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2c0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2c0b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2c0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2c0b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2c0b-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a2c0b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2c0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2c0b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2c0b-116">Not supported.</span></span>|
|<span data-ttu-id="a2c0b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2c0b-117">Application</span></span>|<span data-ttu-id="a2c0b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2c0b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2c0b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2c0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2c0b-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a2c0b-120">Optional query parameters</span></span>
<span data-ttu-id="a2c0b-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a2c0b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2c0b-122">Request headers</span></span>
|<span data-ttu-id="a2c0b-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a2c0b-123">Header</span></span>|<span data-ttu-id="a2c0b-124">Wert</span><span class="sxs-lookup"><span data-stu-id="a2c0b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2c0b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2c0b-125">Authorization</span></span>|<span data-ttu-id="a2c0b-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a2c0b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2c0b-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a2c0b-127">Accept</span></span>|<span data-ttu-id="a2c0b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a2c0b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2c0b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2c0b-129">Request body</span></span>
<span data-ttu-id="a2c0b-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2c0b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2c0b-131">Response</span></span>
<span data-ttu-id="a2c0b-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2c0b-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2c0b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2c0b-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2c0b-134">Request</span></span>
<span data-ttu-id="a2c0b-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="a2c0b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2c0b-136">Response</span></span>
<span data-ttu-id="a2c0b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2c0b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
    "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
    "runState": "success",
    "resultMessage": "Result Message value",
    "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
    "errorCode": 9,
    "errorDescription": "Error Description value"
  }
}
```





