---
title: Aktion „cleanWindowsDevice“
description: Windows-Gerät bereinigen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f97e8b9d9f6095cce7c9dcd9cc4106fda08a7f4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982448"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="36f89-103">cleanWindowsDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="36f89-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="36f89-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="36f89-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36f89-105">Diese Aktion bereinigt Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="36f89-105">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36f89-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36f89-106">Prerequisites</span></span>
<span data-ttu-id="36f89-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36f89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36f89-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36f89-109">Permission type</span></span>|<span data-ttu-id="36f89-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36f89-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36f89-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36f89-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36f89-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="36f89-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="36f89-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36f89-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36f89-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36f89-114">Not supported.</span></span>|
|<span data-ttu-id="36f89-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36f89-115">Application</span></span>|<span data-ttu-id="36f89-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36f89-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36f89-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36f89-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="36f89-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36f89-118">Request headers</span></span>
|<span data-ttu-id="36f89-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="36f89-119">Header</span></span>|<span data-ttu-id="36f89-120">Wert</span><span class="sxs-lookup"><span data-stu-id="36f89-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36f89-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36f89-121">Authorization</span></span>|<span data-ttu-id="36f89-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="36f89-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36f89-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="36f89-123">Accept</span></span>|<span data-ttu-id="36f89-124">application/json</span><span class="sxs-lookup"><span data-stu-id="36f89-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36f89-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36f89-125">Request body</span></span>
<span data-ttu-id="36f89-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="36f89-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="36f89-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="36f89-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="36f89-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36f89-128">Property</span></span>|<span data-ttu-id="36f89-129">Typ</span><span class="sxs-lookup"><span data-stu-id="36f89-129">Type</span></span>|<span data-ttu-id="36f89-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36f89-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36f89-131">keepUserData</span><span class="sxs-lookup"><span data-stu-id="36f89-131">keepUserData</span></span>|<span data-ttu-id="36f89-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="36f89-132">Boolean</span></span>|<span data-ttu-id="36f89-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="36f89-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="36f89-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="36f89-134">Response</span></span>
<span data-ttu-id="36f89-135">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36f89-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="36f89-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36f89-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="36f89-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36f89-137">Request</span></span>
<span data-ttu-id="36f89-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36f89-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="36f89-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="36f89-139">Response</span></span>
<span data-ttu-id="36f89-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36f89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



