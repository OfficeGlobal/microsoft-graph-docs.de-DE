---
title: updateWindowsDeviceAccount-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2990410bbdc343f85f422e1bf40dc1b6fe120864
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954092"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="0e77d-103">updateWindowsDeviceAccount-Aktion</span><span class="sxs-lookup"><span data-stu-id="0e77d-103">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="0e77d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0e77d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e77d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e77d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e77d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0e77d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e77d-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0e77d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e77d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0e77d-108">Prerequisites</span></span>
<span data-ttu-id="0e77d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e77d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e77d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e77d-111">Permission type</span></span>|<span data-ttu-id="0e77d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e77d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e77d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e77d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e77d-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="0e77d-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="0e77d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e77d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e77d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e77d-116">Not supported.</span></span>|
|<span data-ttu-id="0e77d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e77d-117">Application</span></span>|<span data-ttu-id="0e77d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e77d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e77d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e77d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="0e77d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e77d-120">Request headers</span></span>
|<span data-ttu-id="0e77d-121">Header</span><span class="sxs-lookup"><span data-stu-id="0e77d-121">Header</span></span>|<span data-ttu-id="0e77d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0e77d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e77d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e77d-123">Authorization</span></span>|<span data-ttu-id="0e77d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0e77d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e77d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0e77d-125">Accept</span></span>|<span data-ttu-id="0e77d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e77d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e77d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e77d-127">Request body</span></span>
<span data-ttu-id="0e77d-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="0e77d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0e77d-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="0e77d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0e77d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e77d-130">Property</span></span>|<span data-ttu-id="0e77d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0e77d-131">Type</span></span>|<span data-ttu-id="0e77d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e77d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e77d-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="0e77d-133">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="0e77d-134">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="0e77d-134">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="0e77d-135">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0e77d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0e77d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e77d-136">Response</span></span>
<span data-ttu-id="0e77d-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="0e77d-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e77d-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e77d-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e77d-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e77d-139">Request</span></span>
<span data-ttu-id="0e77d-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e77d-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="0e77d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e77d-141">Response</span></span>
<span data-ttu-id="0e77d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e77d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





