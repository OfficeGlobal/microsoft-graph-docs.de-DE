---
title: AssignUserToDevice Aktion
description: Autopilot Geräte Benutzer zugewiesen.
ms.openlocfilehash: 7e3152b4ac158714d37f5d5eb1b830a21dd3745d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061068"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="15f93-103">AssignUserToDevice Aktion</span><span class="sxs-lookup"><span data-stu-id="15f93-103">assignUserToDevice action</span></span>

> <span data-ttu-id="15f93-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="15f93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15f93-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15f93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15f93-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15f93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15f93-107">Autopilot Geräte Benutzer zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="15f93-107">Assigns user to Autopilot devices.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15f93-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15f93-108">Prerequisites</span></span>
<span data-ttu-id="15f93-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15f93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15f93-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15f93-111">Permission type</span></span>|<span data-ttu-id="15f93-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15f93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15f93-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15f93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15f93-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15f93-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15f93-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15f93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15f93-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15f93-116">Not supported.</span></span>|
|<span data-ttu-id="15f93-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15f93-117">Application</span></span>|<span data-ttu-id="15f93-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15f93-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15f93-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15f93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="15f93-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15f93-120">Request headers</span></span>
|<span data-ttu-id="15f93-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="15f93-121">Header</span></span>|<span data-ttu-id="15f93-122">Wert</span><span class="sxs-lookup"><span data-stu-id="15f93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15f93-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15f93-123">Authorization</span></span>|<span data-ttu-id="15f93-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15f93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15f93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15f93-125">Accept</span></span>|<span data-ttu-id="15f93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15f93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15f93-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15f93-127">Request body</span></span>
<span data-ttu-id="15f93-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="15f93-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="15f93-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="15f93-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="15f93-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15f93-130">Property</span></span>|<span data-ttu-id="15f93-131">Typ</span><span class="sxs-lookup"><span data-stu-id="15f93-131">Type</span></span>|<span data-ttu-id="15f93-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15f93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15f93-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="15f93-133">userPrincipalName</span></span>|<span data-ttu-id="15f93-134">String</span><span class="sxs-lookup"><span data-stu-id="15f93-134">String</span></span>|<span data-ttu-id="15f93-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="15f93-135">Not yet documented</span></span>|
|<span data-ttu-id="15f93-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="15f93-136">addressableUserName</span></span>|<span data-ttu-id="15f93-137">String</span><span class="sxs-lookup"><span data-stu-id="15f93-137">String</span></span>|<span data-ttu-id="15f93-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="15f93-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="15f93-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="15f93-139">Response</span></span>
<span data-ttu-id="15f93-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="15f93-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15f93-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15f93-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="15f93-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15f93-142">Request</span></span>
<span data-ttu-id="15f93-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15f93-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="15f93-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="15f93-144">Response</span></span>
<span data-ttu-id="15f93-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15f93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





