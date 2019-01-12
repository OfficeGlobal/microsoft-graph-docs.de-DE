---
title: Aktion „wipe“
description: Mit dieser Aktion lässt sich ein Gerät zurücksetzen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20ebe11dce6847066148f06a77bffa970e3a1b1e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919820"
---
# <a name="wipe-action"></a><span data-ttu-id="4a24c-103">Aktion „wipe“</span><span class="sxs-lookup"><span data-stu-id="4a24c-103">wipe action</span></span>

> <span data-ttu-id="4a24c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4a24c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a24c-105">Mit dieser Aktion lässt sich ein Gerät zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="4a24c-105">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a24c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4a24c-106">Prerequisites</span></span>
<span data-ttu-id="4a24c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a24c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a24c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a24c-109">Permission type</span></span>|<span data-ttu-id="4a24c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a24c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a24c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a24c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4a24c-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4a24c-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="4a24c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a24c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a24c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a24c-114">Not supported.</span></span>|
|<span data-ttu-id="4a24c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a24c-115">Application</span></span>|<span data-ttu-id="4a24c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a24c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a24c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a24c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="4a24c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a24c-118">Request headers</span></span>
|<span data-ttu-id="4a24c-119">Header</span><span class="sxs-lookup"><span data-stu-id="4a24c-119">Header</span></span>|<span data-ttu-id="4a24c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4a24c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a24c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a24c-121">Authorization</span></span>|<span data-ttu-id="4a24c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4a24c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a24c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4a24c-123">Accept</span></span>|<span data-ttu-id="4a24c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4a24c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a24c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a24c-125">Request body</span></span>
<span data-ttu-id="4a24c-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="4a24c-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4a24c-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4a24c-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4a24c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4a24c-128">Property</span></span>|<span data-ttu-id="4a24c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4a24c-129">Type</span></span>|<span data-ttu-id="4a24c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a24c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a24c-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="4a24c-131">keepEnrollmentData</span></span>|<span data-ttu-id="4a24c-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a24c-132">Boolean</span></span>|<span data-ttu-id="4a24c-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4a24c-133">Not yet documented</span></span>|
|<span data-ttu-id="4a24c-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="4a24c-134">keepUserData</span></span>|<span data-ttu-id="4a24c-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4a24c-135">Boolean</span></span>|<span data-ttu-id="4a24c-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4a24c-136">Not yet documented</span></span>|
|<span data-ttu-id="4a24c-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="4a24c-137">macOsUnlockCode</span></span>|<span data-ttu-id="4a24c-138">String</span><span class="sxs-lookup"><span data-stu-id="4a24c-138">String</span></span>|<span data-ttu-id="4a24c-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4a24c-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4a24c-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a24c-140">Response</span></span>
<span data-ttu-id="4a24c-141">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="4a24c-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4a24c-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a24c-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a24c-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a24c-143">Request</span></span>
<span data-ttu-id="4a24c-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a24c-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="4a24c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a24c-145">Response</span></span>
<span data-ttu-id="4a24c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a24c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



