---
title: Aktion „wipe“
description: Mit dieser Aktion lässt sich ein Gerät zurücksetzen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c0d3ce629d27efe481f87a4c88a7c1518889d58c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924965"
---
# <a name="wipe-action"></a><span data-ttu-id="22a00-103">Aktion „wipe“</span><span class="sxs-lookup"><span data-stu-id="22a00-103">wipe action</span></span>

> <span data-ttu-id="22a00-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="22a00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22a00-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="22a00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22a00-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="22a00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22a00-107">Mit dieser Aktion lässt sich ein Gerät zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="22a00-107">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22a00-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="22a00-108">Prerequisites</span></span>
<span data-ttu-id="22a00-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22a00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22a00-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22a00-111">Permission type</span></span>|<span data-ttu-id="22a00-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22a00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22a00-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22a00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22a00-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="22a00-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="22a00-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22a00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22a00-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22a00-116">Not supported.</span></span>|
|<span data-ttu-id="22a00-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22a00-117">Application</span></span>|<span data-ttu-id="22a00-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22a00-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22a00-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22a00-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="22a00-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22a00-120">Request headers</span></span>
|<span data-ttu-id="22a00-121">Header</span><span class="sxs-lookup"><span data-stu-id="22a00-121">Header</span></span>|<span data-ttu-id="22a00-122">Wert</span><span class="sxs-lookup"><span data-stu-id="22a00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22a00-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22a00-123">Authorization</span></span>|<span data-ttu-id="22a00-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="22a00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22a00-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="22a00-125">Accept</span></span>|<span data-ttu-id="22a00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22a00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22a00-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22a00-127">Request body</span></span>
<span data-ttu-id="22a00-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="22a00-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="22a00-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="22a00-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="22a00-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="22a00-130">Property</span></span>|<span data-ttu-id="22a00-131">Typ</span><span class="sxs-lookup"><span data-stu-id="22a00-131">Type</span></span>|<span data-ttu-id="22a00-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22a00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22a00-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="22a00-133">keepEnrollmentData</span></span>|<span data-ttu-id="22a00-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a00-134">Boolean</span></span>|<span data-ttu-id="22a00-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="22a00-135">Not yet documented</span></span>|
|<span data-ttu-id="22a00-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="22a00-136">keepUserData</span></span>|<span data-ttu-id="22a00-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="22a00-137">Boolean</span></span>|<span data-ttu-id="22a00-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="22a00-138">Not yet documented</span></span>|
|<span data-ttu-id="22a00-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="22a00-139">macOsUnlockCode</span></span>|<span data-ttu-id="22a00-140">String</span><span class="sxs-lookup"><span data-stu-id="22a00-140">String</span></span>|<span data-ttu-id="22a00-141">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="22a00-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="22a00-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="22a00-142">Response</span></span>
<span data-ttu-id="22a00-143">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="22a00-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="22a00-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22a00-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="22a00-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22a00-145">Request</span></span>
<span data-ttu-id="22a00-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22a00-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22a00-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="22a00-147">Response</span></span>
<span data-ttu-id="22a00-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22a00-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





