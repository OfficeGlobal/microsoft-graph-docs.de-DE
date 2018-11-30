---
title: rebootNow-Aktion
description: Gerät neu starten
ms.openlocfilehash: 03da8e4781302a11e10f20df2404764e0d0f05a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065320"
---
# <a name="rebootnow-action"></a><span data-ttu-id="b1acb-103">rebootNow-Aktion</span><span class="sxs-lookup"><span data-stu-id="b1acb-103">rebootNow action</span></span>

> <span data-ttu-id="b1acb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1acb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1acb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1acb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1acb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b1acb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1acb-107">Gerät neu starten</span><span class="sxs-lookup"><span data-stu-id="b1acb-107">Reboot device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1acb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b1acb-108">Prerequisites</span></span>
<span data-ttu-id="b1acb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1acb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1acb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1acb-111">Permission type</span></span>|<span data-ttu-id="b1acb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1acb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1acb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1acb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1acb-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b1acb-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="b1acb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1acb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1acb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1acb-116">Not supported.</span></span>|
|<span data-ttu-id="b1acb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1acb-117">Application</span></span>|<span data-ttu-id="b1acb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1acb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1acb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1acb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rebootNow
```

## <a name="request-headers"></a><span data-ttu-id="b1acb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1acb-120">Request headers</span></span>
|<span data-ttu-id="b1acb-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b1acb-121">Header</span></span>|<span data-ttu-id="b1acb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b1acb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1acb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1acb-123">Authorization</span></span>|<span data-ttu-id="b1acb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b1acb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1acb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1acb-125">Accept</span></span>|<span data-ttu-id="b1acb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1acb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1acb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1acb-127">Request body</span></span>
<span data-ttu-id="b1acb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b1acb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1acb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1acb-129">Response</span></span>
<span data-ttu-id="b1acb-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="b1acb-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1acb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1acb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1acb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1acb-132">Request</span></span>
<span data-ttu-id="b1acb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1acb-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/rebootNow
```

### <a name="response"></a><span data-ttu-id="b1acb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1acb-134">Response</span></span>
<span data-ttu-id="b1acb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1acb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





