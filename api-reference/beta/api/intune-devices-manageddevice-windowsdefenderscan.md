---
title: windowsDefenderScan-Aktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae19e2977c50502fab91bea7d9fda751d1501b0c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966985"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="cbced-103">windowsDefenderScan-Aktion</span><span class="sxs-lookup"><span data-stu-id="cbced-103">windowsDefenderScan action</span></span>

> <span data-ttu-id="cbced-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cbced-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbced-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cbced-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbced-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="cbced-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbced-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cbced-107">Prerequisites</span></span>
<span data-ttu-id="cbced-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbced-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cbced-110">Permission type</span></span>|<span data-ttu-id="cbced-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cbced-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbced-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cbced-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbced-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="cbced-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="cbced-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cbced-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbced-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbced-115">Not supported.</span></span>|
|<span data-ttu-id="cbced-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cbced-116">Application</span></span>|<span data-ttu-id="cbced-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbced-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbced-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbced-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="cbced-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cbced-119">Request headers</span></span>
|<span data-ttu-id="cbced-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cbced-120">Header</span></span>|<span data-ttu-id="cbced-121">Wert</span><span class="sxs-lookup"><span data-stu-id="cbced-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbced-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbced-122">Authorization</span></span>|<span data-ttu-id="cbced-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cbced-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbced-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cbced-124">Accept</span></span>|<span data-ttu-id="cbced-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbced-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbced-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cbced-126">Request body</span></span>
<span data-ttu-id="cbced-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="cbced-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cbced-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="cbced-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cbced-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cbced-129">Property</span></span>|<span data-ttu-id="cbced-130">Typ</span><span class="sxs-lookup"><span data-stu-id="cbced-130">Type</span></span>|<span data-ttu-id="cbced-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbced-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbced-132">quickScan</span><span class="sxs-lookup"><span data-stu-id="cbced-132">quickScan</span></span>|<span data-ttu-id="cbced-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbced-133">Boolean</span></span>|<span data-ttu-id="cbced-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="cbced-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cbced-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbced-135">Response</span></span>
<span data-ttu-id="cbced-136">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbced-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cbced-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cbced-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbced-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbced-138">Request</span></span>
<span data-ttu-id="cbced-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cbced-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="cbced-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbced-140">Response</span></span>
<span data-ttu-id="cbced-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbced-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




