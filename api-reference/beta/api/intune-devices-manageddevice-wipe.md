---
title: Aktion „wipe“
description: Mit dieser Aktion lässt sich ein Gerät zurücksetzen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2979333890626d197e596d6e768ac26205888276
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139361"
---
# <a name="wipe-action"></a><span data-ttu-id="32ee9-103">Zurücksetzung</span><span class="sxs-lookup"><span data-stu-id="32ee9-103">wipe action</span></span>

> <span data-ttu-id="32ee9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="32ee9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32ee9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="32ee9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32ee9-106">Mit dieser Aktion lässt sich ein Gerät zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="32ee9-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32ee9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="32ee9-107">Prerequisites</span></span>
<span data-ttu-id="32ee9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="32ee9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="32ee9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32ee9-110">Permission type</span></span>|<span data-ttu-id="32ee9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32ee9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32ee9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32ee9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32ee9-113">DeviceManagementManagedDevices. PriviligedOperation. all, DeviceManagementManagedDevices. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="32ee9-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="32ee9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32ee9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32ee9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32ee9-115">Not supported.</span></span>|
|<span data-ttu-id="32ee9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32ee9-116">Application</span></span>|<span data-ttu-id="32ee9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32ee9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32ee9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32ee9-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="32ee9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32ee9-119">Request headers</span></span>
|<span data-ttu-id="32ee9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="32ee9-120">Header</span></span>|<span data-ttu-id="32ee9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="32ee9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32ee9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32ee9-122">Authorization</span></span>|<span data-ttu-id="32ee9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="32ee9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32ee9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="32ee9-124">Accept</span></span>|<span data-ttu-id="32ee9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32ee9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32ee9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32ee9-126">Request body</span></span>
<span data-ttu-id="32ee9-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="32ee9-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="32ee9-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="32ee9-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="32ee9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32ee9-129">Property</span></span>|<span data-ttu-id="32ee9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="32ee9-130">Type</span></span>|<span data-ttu-id="32ee9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32ee9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32ee9-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="32ee9-132">keepEnrollmentData</span></span>|<span data-ttu-id="32ee9-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="32ee9-133">Boolean</span></span>|<span data-ttu-id="32ee9-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="32ee9-134">Not yet documented</span></span>|
|<span data-ttu-id="32ee9-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="32ee9-135">keepUserData</span></span>|<span data-ttu-id="32ee9-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="32ee9-136">Boolean</span></span>|<span data-ttu-id="32ee9-137">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="32ee9-137">Not yet documented</span></span>|
|<span data-ttu-id="32ee9-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="32ee9-138">macOsUnlockCode</span></span>|<span data-ttu-id="32ee9-139">String</span><span class="sxs-lookup"><span data-stu-id="32ee9-139">String</span></span>|<span data-ttu-id="32ee9-140">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="32ee9-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="32ee9-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="32ee9-141">Response</span></span>
<span data-ttu-id="32ee9-142">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="32ee9-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32ee9-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32ee9-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="32ee9-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32ee9-144">Request</span></span>
<span data-ttu-id="32ee9-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32ee9-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32ee9-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="32ee9-146">Response</span></span>
<span data-ttu-id="32ee9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32ee9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




