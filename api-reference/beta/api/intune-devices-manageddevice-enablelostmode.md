---
title: EnableLostMode Aktion
description: Verloren-Modus aktivieren
author: tfitzmac
ms.openlocfilehash: b75df200a57f5861515f1e5d3c867df8b3f08276
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359479"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="3b407-103">EnableLostMode Aktion</span><span class="sxs-lookup"><span data-stu-id="3b407-103">enableLostMode action</span></span>

> <span data-ttu-id="3b407-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b407-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b407-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b407-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b407-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3b407-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b407-107">Verloren-Modus aktivieren</span><span class="sxs-lookup"><span data-stu-id="3b407-107">Enable lost mode</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b407-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3b407-108">Prerequisites</span></span>
<span data-ttu-id="3b407-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b407-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b407-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b407-111">Permission type</span></span>|<span data-ttu-id="3b407-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b407-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b407-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b407-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b407-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3b407-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="3b407-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b407-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b407-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b407-116">Not supported.</span></span>|
|<span data-ttu-id="3b407-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b407-117">Application</span></span>|<span data-ttu-id="3b407-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b407-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b407-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b407-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="3b407-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b407-120">Request headers</span></span>
|<span data-ttu-id="3b407-121">Header</span><span class="sxs-lookup"><span data-stu-id="3b407-121">Header</span></span>|<span data-ttu-id="3b407-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3b407-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b407-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3b407-123">Authorization</span></span>|<span data-ttu-id="3b407-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3b407-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b407-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b407-125">Accept</span></span>|<span data-ttu-id="3b407-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b407-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b407-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b407-127">Request body</span></span>
<span data-ttu-id="3b407-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="3b407-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3b407-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="3b407-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3b407-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b407-130">Property</span></span>|<span data-ttu-id="3b407-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3b407-131">Type</span></span>|<span data-ttu-id="3b407-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b407-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b407-133">message</span><span class="sxs-lookup"><span data-stu-id="3b407-133">message</span></span>|<span data-ttu-id="3b407-134">String</span><span class="sxs-lookup"><span data-stu-id="3b407-134">String</span></span>|<span data-ttu-id="3b407-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3b407-135">Not yet documented</span></span>|
|<span data-ttu-id="3b407-136">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="3b407-136">phoneNumber</span></span>|<span data-ttu-id="3b407-137">String</span><span class="sxs-lookup"><span data-stu-id="3b407-137">String</span></span>|<span data-ttu-id="3b407-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3b407-138">Not yet documented</span></span>|
|<span data-ttu-id="3b407-139">Fußzeile</span><span class="sxs-lookup"><span data-stu-id="3b407-139">footer</span></span>|<span data-ttu-id="3b407-140">String</span><span class="sxs-lookup"><span data-stu-id="3b407-140">String</span></span>|<span data-ttu-id="3b407-141">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3b407-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3b407-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b407-142">Response</span></span>
<span data-ttu-id="3b407-143">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="3b407-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3b407-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b407-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b407-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b407-145">Request</span></span>
<span data-ttu-id="3b407-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b407-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="3b407-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b407-147">Response</span></span>
<span data-ttu-id="3b407-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b407-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





