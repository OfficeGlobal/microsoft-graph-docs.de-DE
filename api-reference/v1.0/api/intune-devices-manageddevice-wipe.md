---
title: Aktion „wipe“
description: Mit dieser Aktion lässt sich ein Gerät zurücksetzen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23d4d9536c57d4a9f2af863473b85d2062a06b3a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259157"
---
# <a name="wipe-action"></a><span data-ttu-id="1aca7-103">Zurücksetzung</span><span class="sxs-lookup"><span data-stu-id="1aca7-103">wipe action</span></span>

> <span data-ttu-id="1aca7-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1aca7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aca7-105">Mit dieser Aktion lässt sich ein Gerät zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="1aca7-105">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1aca7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1aca7-106">Prerequisites</span></span>
<span data-ttu-id="1aca7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1aca7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1aca7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1aca7-109">Permission type</span></span>|<span data-ttu-id="1aca7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1aca7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aca7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1aca7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1aca7-112">DeviceManagementManagedDevices. PriviligedOperation. all, DeviceManagementManagedDevices. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="1aca7-112">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1aca7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1aca7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aca7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1aca7-114">Not supported.</span></span>|
|<span data-ttu-id="1aca7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1aca7-115">Application</span></span>|<span data-ttu-id="1aca7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1aca7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aca7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1aca7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="1aca7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1aca7-118">Request headers</span></span>
|<span data-ttu-id="1aca7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1aca7-119">Header</span></span>|<span data-ttu-id="1aca7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1aca7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1aca7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aca7-121">Authorization</span></span>|<span data-ttu-id="1aca7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1aca7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1aca7-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1aca7-123">Accept</span></span>|<span data-ttu-id="1aca7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1aca7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aca7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1aca7-125">Request body</span></span>
<span data-ttu-id="1aca7-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="1aca7-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1aca7-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="1aca7-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1aca7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1aca7-128">Property</span></span>|<span data-ttu-id="1aca7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1aca7-129">Type</span></span>|<span data-ttu-id="1aca7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1aca7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aca7-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="1aca7-131">keepEnrollmentData</span></span>|<span data-ttu-id="1aca7-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca7-132">Boolean</span></span>|<span data-ttu-id="1aca7-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1aca7-133">Not yet documented</span></span>|
|<span data-ttu-id="1aca7-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="1aca7-134">keepUserData</span></span>|<span data-ttu-id="1aca7-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca7-135">Boolean</span></span>|<span data-ttu-id="1aca7-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1aca7-136">Not yet documented</span></span>|
|<span data-ttu-id="1aca7-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="1aca7-137">macOsUnlockCode</span></span>|<span data-ttu-id="1aca7-138">String</span><span class="sxs-lookup"><span data-stu-id="1aca7-138">String</span></span>|<span data-ttu-id="1aca7-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1aca7-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1aca7-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1aca7-140">Response</span></span>
<span data-ttu-id="1aca7-141">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="1aca7-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1aca7-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1aca7-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="1aca7-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1aca7-143">Request</span></span>
<span data-ttu-id="1aca7-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1aca7-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1aca7-145">Reaktion</span><span class="sxs-lookup"><span data-stu-id="1aca7-145">Response</span></span>
<span data-ttu-id="1aca7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1aca7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



