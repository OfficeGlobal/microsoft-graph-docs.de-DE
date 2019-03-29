---
title: Aktion „wipe“
description: Zurücksetzen eines Geräts
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53b21cd7998d8a806fc9cba5aa911573947f5e1b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978395"
---
# <a name="wipe-action"></a><span data-ttu-id="023cc-103">Zurücksetzung</span><span class="sxs-lookup"><span data-stu-id="023cc-103">wipe action</span></span>

> <span data-ttu-id="023cc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="023cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="023cc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="023cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="023cc-106">Mit dieser Aktion lässt sich ein Gerät zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="023cc-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="023cc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="023cc-107">Prerequisites</span></span>
<span data-ttu-id="023cc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="023cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="023cc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="023cc-110">Permission type</span></span>|<span data-ttu-id="023cc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="023cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="023cc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="023cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="023cc-113">DeviceManagementManagedDevices. PriviligedOperation. all, DeviceManagementManagedDevices. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="023cc-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="023cc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="023cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="023cc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="023cc-115">Not supported.</span></span>|
|<span data-ttu-id="023cc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="023cc-116">Application</span></span>|<span data-ttu-id="023cc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="023cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="023cc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="023cc-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="023cc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="023cc-119">Request headers</span></span>
|<span data-ttu-id="023cc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="023cc-120">Header</span></span>|<span data-ttu-id="023cc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="023cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="023cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="023cc-122">Authorization</span></span>|<span data-ttu-id="023cc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="023cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="023cc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="023cc-124">Accept</span></span>|<span data-ttu-id="023cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="023cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="023cc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="023cc-126">Request body</span></span>
<span data-ttu-id="023cc-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="023cc-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="023cc-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="023cc-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="023cc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="023cc-129">Property</span></span>|<span data-ttu-id="023cc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="023cc-130">Type</span></span>|<span data-ttu-id="023cc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="023cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="023cc-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="023cc-132">keepEnrollmentData</span></span>|<span data-ttu-id="023cc-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="023cc-133">Boolean</span></span>|<span data-ttu-id="023cc-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="023cc-134">Not yet documented</span></span>|
|<span data-ttu-id="023cc-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="023cc-135">keepUserData</span></span>|<span data-ttu-id="023cc-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="023cc-136">Boolean</span></span>|<span data-ttu-id="023cc-137">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="023cc-137">Not yet documented</span></span>|
|<span data-ttu-id="023cc-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="023cc-138">macOsUnlockCode</span></span>|<span data-ttu-id="023cc-139">String</span><span class="sxs-lookup"><span data-stu-id="023cc-139">String</span></span>|<span data-ttu-id="023cc-140">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="023cc-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="023cc-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="023cc-141">Response</span></span>
<span data-ttu-id="023cc-142">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="023cc-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="023cc-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="023cc-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="023cc-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="023cc-144">Request</span></span>
<span data-ttu-id="023cc-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="023cc-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="023cc-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="023cc-146">Response</span></span>
<span data-ttu-id="023cc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="023cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




