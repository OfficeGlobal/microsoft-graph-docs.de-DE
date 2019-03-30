---
title: Aktion „wipe“
description: Zurücksetzen eines Geräts
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3249421de530cdc8e5e7f9c5a90676572c5b7ae9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983232"
---
# <a name="wipe-action"></a><span data-ttu-id="603d5-103">Zurücksetzung</span><span class="sxs-lookup"><span data-stu-id="603d5-103">wipe action</span></span>

> <span data-ttu-id="603d5-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="603d5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="603d5-105">Mit dieser Aktion lässt sich ein Gerät zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="603d5-105">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="603d5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="603d5-106">Prerequisites</span></span>
<span data-ttu-id="603d5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="603d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="603d5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="603d5-109">Permission type</span></span>|<span data-ttu-id="603d5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="603d5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="603d5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="603d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="603d5-112">DeviceManagementManagedDevices. PriviligedOperation. all, DeviceManagementManagedDevices. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="603d5-112">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="603d5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="603d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="603d5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="603d5-114">Not supported.</span></span>|
|<span data-ttu-id="603d5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="603d5-115">Application</span></span>|<span data-ttu-id="603d5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="603d5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="603d5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="603d5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="603d5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="603d5-118">Request headers</span></span>
|<span data-ttu-id="603d5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="603d5-119">Header</span></span>|<span data-ttu-id="603d5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="603d5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="603d5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="603d5-121">Authorization</span></span>|<span data-ttu-id="603d5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="603d5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="603d5-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="603d5-123">Accept</span></span>|<span data-ttu-id="603d5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="603d5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="603d5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="603d5-125">Request body</span></span>
<span data-ttu-id="603d5-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="603d5-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="603d5-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="603d5-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="603d5-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="603d5-128">Property</span></span>|<span data-ttu-id="603d5-129">Typ</span><span class="sxs-lookup"><span data-stu-id="603d5-129">Type</span></span>|<span data-ttu-id="603d5-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="603d5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="603d5-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="603d5-131">keepEnrollmentData</span></span>|<span data-ttu-id="603d5-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="603d5-132">Boolean</span></span>|<span data-ttu-id="603d5-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="603d5-133">Not yet documented</span></span>|
|<span data-ttu-id="603d5-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="603d5-134">keepUserData</span></span>|<span data-ttu-id="603d5-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="603d5-135">Boolean</span></span>|<span data-ttu-id="603d5-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="603d5-136">Not yet documented</span></span>|
|<span data-ttu-id="603d5-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="603d5-137">macOsUnlockCode</span></span>|<span data-ttu-id="603d5-138">String</span><span class="sxs-lookup"><span data-stu-id="603d5-138">String</span></span>|<span data-ttu-id="603d5-139">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="603d5-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="603d5-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="603d5-140">Response</span></span>
<span data-ttu-id="603d5-141">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="603d5-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="603d5-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="603d5-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="603d5-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="603d5-143">Request</span></span>
<span data-ttu-id="603d5-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="603d5-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="603d5-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="603d5-145">Response</span></span>
<span data-ttu-id="603d5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="603d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



