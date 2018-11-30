---
title: remoteLock-Aktion
description: Remotesperre
ms.openlocfilehash: de94140e1c4d8a7214af63bd3b6d884d312c24fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062006"
---
# <a name="remotelock-action"></a><span data-ttu-id="e60d2-103">remoteLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="e60d2-103">remoteLock action</span></span>

> <span data-ttu-id="e60d2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e60d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e60d2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e60d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e60d2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e60d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e60d2-107">Remotesperre</span><span class="sxs-lookup"><span data-stu-id="e60d2-107">Remote lock</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e60d2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e60d2-108">Prerequisites</span></span>
<span data-ttu-id="e60d2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e60d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e60d2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e60d2-111">Permission type</span></span>|<span data-ttu-id="e60d2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e60d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e60d2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e60d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e60d2-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e60d2-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e60d2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e60d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e60d2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e60d2-116">Not supported.</span></span>|
|<span data-ttu-id="e60d2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e60d2-117">Application</span></span>|<span data-ttu-id="e60d2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e60d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e60d2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e60d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="e60d2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e60d2-120">Request headers</span></span>
|<span data-ttu-id="e60d2-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e60d2-121">Header</span></span>|<span data-ttu-id="e60d2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e60d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e60d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e60d2-123">Authorization</span></span>|<span data-ttu-id="e60d2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e60d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e60d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e60d2-125">Accept</span></span>|<span data-ttu-id="e60d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e60d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e60d2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e60d2-127">Request body</span></span>
<span data-ttu-id="e60d2-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e60d2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e60d2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e60d2-129">Response</span></span>
<span data-ttu-id="e60d2-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="e60d2-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e60d2-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e60d2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e60d2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e60d2-132">Request</span></span>
<span data-ttu-id="e60d2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e60d2-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="e60d2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e60d2-134">Response</span></span>
<span data-ttu-id="e60d2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e60d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





