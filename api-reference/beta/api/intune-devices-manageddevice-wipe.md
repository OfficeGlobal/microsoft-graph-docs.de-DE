---
title: Aktion „wipe“
description: Mit dieser Aktion lässt sich ein Gerät zurücksetzen.
ms.openlocfilehash: 841a0c5e968cb3fa9816b604cc3d2e335ca75a4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061715"
---
# <a name="wipe-action"></a><span data-ttu-id="87f43-103">Aktion „wipe“</span><span class="sxs-lookup"><span data-stu-id="87f43-103">wipe action</span></span>

> <span data-ttu-id="87f43-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87f43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87f43-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87f43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87f43-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="87f43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87f43-107">Mit dieser Aktion lässt sich ein Gerät zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="87f43-107">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87f43-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="87f43-108">Prerequisites</span></span>
<span data-ttu-id="87f43-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87f43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87f43-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87f43-111">Permission type</span></span>|<span data-ttu-id="87f43-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87f43-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87f43-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87f43-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87f43-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="87f43-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="87f43-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87f43-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87f43-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87f43-116">Not supported.</span></span>|
|<span data-ttu-id="87f43-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87f43-117">Application</span></span>|<span data-ttu-id="87f43-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87f43-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87f43-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87f43-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="87f43-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87f43-120">Request headers</span></span>
|<span data-ttu-id="87f43-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="87f43-121">Header</span></span>|<span data-ttu-id="87f43-122">Wert</span><span class="sxs-lookup"><span data-stu-id="87f43-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87f43-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87f43-123">Authorization</span></span>|<span data-ttu-id="87f43-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="87f43-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87f43-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87f43-125">Accept</span></span>|<span data-ttu-id="87f43-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87f43-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87f43-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87f43-127">Request body</span></span>
<span data-ttu-id="87f43-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="87f43-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="87f43-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="87f43-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="87f43-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87f43-130">Property</span></span>|<span data-ttu-id="87f43-131">Typ</span><span class="sxs-lookup"><span data-stu-id="87f43-131">Type</span></span>|<span data-ttu-id="87f43-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87f43-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87f43-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="87f43-133">keepEnrollmentData</span></span>|<span data-ttu-id="87f43-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="87f43-134">Boolean</span></span>|<span data-ttu-id="87f43-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="87f43-135">Not yet documented</span></span>|
|<span data-ttu-id="87f43-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="87f43-136">keepUserData</span></span>|<span data-ttu-id="87f43-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="87f43-137">Boolean</span></span>|<span data-ttu-id="87f43-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="87f43-138">Not yet documented</span></span>|
|<span data-ttu-id="87f43-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="87f43-139">macOsUnlockCode</span></span>|<span data-ttu-id="87f43-140">String</span><span class="sxs-lookup"><span data-stu-id="87f43-140">String</span></span>|<span data-ttu-id="87f43-141">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="87f43-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="87f43-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="87f43-142">Response</span></span>
<span data-ttu-id="87f43-143">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="87f43-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="87f43-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87f43-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="87f43-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87f43-145">Request</span></span>
<span data-ttu-id="87f43-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87f43-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="87f43-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="87f43-147">Response</span></span>
<span data-ttu-id="87f43-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87f43-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





