---
title: AssignUserToDevice Aktion
description: Autopilot Geräte Benutzer zugewiesen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3c91107ade1ce04a1aef9bac0876335ca2093555
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979530"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="b9dd5-103">AssignUserToDevice Aktion</span><span class="sxs-lookup"><span data-stu-id="b9dd5-103">assignUserToDevice action</span></span>

> <span data-ttu-id="b9dd5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9dd5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9dd5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9dd5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9dd5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b9dd5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9dd5-107">Autopilot Geräte Benutzer zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="b9dd5-107">Assigns user to Autopilot devices.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9dd5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9dd5-108">Prerequisites</span></span>
<span data-ttu-id="b9dd5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9dd5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9dd5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9dd5-111">Permission type</span></span>|<span data-ttu-id="b9dd5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9dd5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9dd5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9dd5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9dd5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9dd5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b9dd5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9dd5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9dd5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9dd5-116">Not supported.</span></span>|
|<span data-ttu-id="b9dd5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9dd5-117">Application</span></span>|<span data-ttu-id="b9dd5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9dd5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9dd5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9dd5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="b9dd5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9dd5-120">Request headers</span></span>
|<span data-ttu-id="b9dd5-121">Header</span><span class="sxs-lookup"><span data-stu-id="b9dd5-121">Header</span></span>|<span data-ttu-id="b9dd5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b9dd5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9dd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9dd5-123">Authorization</span></span>|<span data-ttu-id="b9dd5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9dd5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9dd5-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b9dd5-125">Accept</span></span>|<span data-ttu-id="b9dd5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9dd5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9dd5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9dd5-127">Request body</span></span>
<span data-ttu-id="b9dd5-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="b9dd5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b9dd5-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b9dd5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b9dd5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9dd5-130">Property</span></span>|<span data-ttu-id="b9dd5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b9dd5-131">Type</span></span>|<span data-ttu-id="b9dd5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9dd5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9dd5-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9dd5-133">userPrincipalName</span></span>|<span data-ttu-id="b9dd5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9dd5-134">String</span></span>|<span data-ttu-id="b9dd5-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b9dd5-135">Not yet documented</span></span>|
|<span data-ttu-id="b9dd5-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="b9dd5-136">addressableUserName</span></span>|<span data-ttu-id="b9dd5-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9dd5-137">String</span></span>|<span data-ttu-id="b9dd5-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b9dd5-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b9dd5-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9dd5-139">Response</span></span>
<span data-ttu-id="b9dd5-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="b9dd5-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b9dd5-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9dd5-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9dd5-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9dd5-142">Request</span></span>
<span data-ttu-id="b9dd5-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9dd5-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="b9dd5-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9dd5-144">Response</span></span>
<span data-ttu-id="b9dd5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9dd5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





