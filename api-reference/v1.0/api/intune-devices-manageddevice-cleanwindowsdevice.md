---
title: Aktion „cleanWindowsDevice“
description: Diese Aktion bereinigt Windows-Geräte.
ms.openlocfilehash: bf454ddac63c22fb581b6c52476c8a4918ed6110
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016158"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="2bebe-103">Aktion „cleanWindowsDevice“</span><span class="sxs-lookup"><span data-stu-id="2bebe-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="2bebe-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2bebe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2bebe-105">Diese Aktion bereinigt Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="2bebe-105">Clean Windows device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2bebe-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2bebe-106">Prerequisites</span></span>
<span data-ttu-id="2bebe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bebe-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2bebe-109">Permission type</span></span>|<span data-ttu-id="2bebe-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2bebe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bebe-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2bebe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2bebe-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2bebe-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="2bebe-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2bebe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bebe-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2bebe-114">Not supported.</span></span>|
|<span data-ttu-id="2bebe-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2bebe-115">Application</span></span>|<span data-ttu-id="2bebe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2bebe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bebe-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2bebe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="2bebe-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2bebe-118">Request headers</span></span>
|<span data-ttu-id="2bebe-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2bebe-119">Header</span></span>|<span data-ttu-id="2bebe-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2bebe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bebe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bebe-121">Authorization</span></span>|<span data-ttu-id="2bebe-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2bebe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bebe-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2bebe-123">Accept</span></span>|<span data-ttu-id="2bebe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2bebe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bebe-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2bebe-125">Request body</span></span>
<span data-ttu-id="2bebe-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="2bebe-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2bebe-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="2bebe-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2bebe-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2bebe-128">Property</span></span>|<span data-ttu-id="2bebe-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2bebe-129">Type</span></span>|<span data-ttu-id="2bebe-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2bebe-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bebe-131">keepUserData</span><span class="sxs-lookup"><span data-stu-id="2bebe-131">keepUserData</span></span>|<span data-ttu-id="2bebe-132">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2bebe-132">Boolean</span></span>|<span data-ttu-id="2bebe-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2bebe-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2bebe-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2bebe-134">Response</span></span>
<span data-ttu-id="2bebe-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="2bebe-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2bebe-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2bebe-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="2bebe-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2bebe-137">Request</span></span>
<span data-ttu-id="2bebe-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2bebe-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="2bebe-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="2bebe-139">Response</span></span>
<span data-ttu-id="2bebe-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2bebe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



