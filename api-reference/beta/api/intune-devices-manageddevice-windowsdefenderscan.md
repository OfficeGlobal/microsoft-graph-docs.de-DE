---
title: windowsDefenderScan-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6a3ac226f5169f96f87186bdde2cc54a5c55e651
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915872"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="f621b-103">windowsDefenderScan-Aktion</span><span class="sxs-lookup"><span data-stu-id="f621b-103">windowsDefenderScan action</span></span>

> <span data-ttu-id="f621b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f621b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f621b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f621b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f621b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f621b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f621b-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f621b-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f621b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f621b-108">Prerequisites</span></span>
<span data-ttu-id="f621b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f621b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f621b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f621b-111">Permission type</span></span>|<span data-ttu-id="f621b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f621b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f621b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f621b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f621b-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f621b-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="f621b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f621b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f621b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f621b-116">Not supported.</span></span>|
|<span data-ttu-id="f621b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f621b-117">Application</span></span>|<span data-ttu-id="f621b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f621b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f621b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f621b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f621b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f621b-120">Request headers</span></span>
|<span data-ttu-id="f621b-121">Header</span><span class="sxs-lookup"><span data-stu-id="f621b-121">Header</span></span>|<span data-ttu-id="f621b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f621b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f621b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f621b-123">Authorization</span></span>|<span data-ttu-id="f621b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f621b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f621b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f621b-125">Accept</span></span>|<span data-ttu-id="f621b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f621b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f621b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f621b-127">Request body</span></span>
<span data-ttu-id="f621b-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="f621b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f621b-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f621b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f621b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f621b-130">Property</span></span>|<span data-ttu-id="f621b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f621b-131">Type</span></span>|<span data-ttu-id="f621b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f621b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f621b-133">quickScan</span><span class="sxs-lookup"><span data-stu-id="f621b-133">quickScan</span></span>|<span data-ttu-id="f621b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="f621b-134">Boolean</span></span>|<span data-ttu-id="f621b-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f621b-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f621b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f621b-136">Response</span></span>
<span data-ttu-id="f621b-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="f621b-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f621b-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f621b-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="f621b-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f621b-139">Request</span></span>
<span data-ttu-id="f621b-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f621b-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="f621b-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f621b-141">Response</span></span>
<span data-ttu-id="f621b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f621b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





