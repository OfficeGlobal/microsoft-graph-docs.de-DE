---
title: Aktion „wipe“
description: Mit dieser Aktion lässt sich ein Gerät zurücksetzen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 56ee058ee4ea6c5760707f895d626b35163c68ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398709"
---
# <a name="wipe-action"></a><span data-ttu-id="1fb7a-103">Aktion „wipe“</span><span class="sxs-lookup"><span data-stu-id="1fb7a-103">wipe action</span></span>

> <span data-ttu-id="1fb7a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1fb7a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1fb7a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fb7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fb7a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1fb7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fb7a-107">Mit dieser Aktion lässt sich ein Gerät zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="1fb7a-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fb7a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1fb7a-108">Prerequisites</span></span>
<span data-ttu-id="1fb7a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1fb7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1fb7a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1fb7a-111">Permission type</span></span>|<span data-ttu-id="1fb7a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1fb7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fb7a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1fb7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fb7a-114">DeviceManagementManagedDevices.PriviligedOperation.All DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fb7a-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1fb7a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1fb7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fb7a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1fb7a-116">Not supported.</span></span>|
|<span data-ttu-id="1fb7a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1fb7a-117">Application</span></span>|<span data-ttu-id="1fb7a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1fb7a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fb7a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1fb7a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1fb7a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1fb7a-120">Request headers</span></span>
|<span data-ttu-id="1fb7a-121">Header</span><span class="sxs-lookup"><span data-stu-id="1fb7a-121">Header</span></span>|<span data-ttu-id="1fb7a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1fb7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fb7a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1fb7a-123">Authorization</span></span>|<span data-ttu-id="1fb7a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1fb7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fb7a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1fb7a-125">Accept</span></span>|<span data-ttu-id="1fb7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fb7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fb7a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1fb7a-127">Request body</span></span>
<span data-ttu-id="1fb7a-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="1fb7a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1fb7a-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="1fb7a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1fb7a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1fb7a-130">Property</span></span>|<span data-ttu-id="1fb7a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1fb7a-131">Type</span></span>|<span data-ttu-id="1fb7a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1fb7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fb7a-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="1fb7a-133">keepEnrollmentData</span></span>|<span data-ttu-id="1fb7a-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fb7a-134">Boolean</span></span>|<span data-ttu-id="1fb7a-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1fb7a-135">Not yet documented</span></span>|
|<span data-ttu-id="1fb7a-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="1fb7a-136">keepUserData</span></span>|<span data-ttu-id="1fb7a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fb7a-137">Boolean</span></span>|<span data-ttu-id="1fb7a-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1fb7a-138">Not yet documented</span></span>|
|<span data-ttu-id="1fb7a-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="1fb7a-139">macOsUnlockCode</span></span>|<span data-ttu-id="1fb7a-140">String</span><span class="sxs-lookup"><span data-stu-id="1fb7a-140">String</span></span>|<span data-ttu-id="1fb7a-141">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1fb7a-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1fb7a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="1fb7a-142">Response</span></span>
<span data-ttu-id="1fb7a-143">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="1fb7a-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1fb7a-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1fb7a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fb7a-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1fb7a-145">Request</span></span>
<span data-ttu-id="1fb7a-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1fb7a-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1fb7a-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="1fb7a-147">Response</span></span>
<span data-ttu-id="1fb7a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1fb7a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




