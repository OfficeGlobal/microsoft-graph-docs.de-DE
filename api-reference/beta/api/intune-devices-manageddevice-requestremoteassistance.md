---
title: requestRemoteAssistance-Aktion
description: Remoteunterstützung anfordern
ms.openlocfilehash: b33b8ef0c9af355325d2d27d0db476338766c741
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064403"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="8d6ca-103">requestRemoteAssistance-Aktion</span><span class="sxs-lookup"><span data-stu-id="8d6ca-103">requestRemoteAssistance action</span></span>

> <span data-ttu-id="8d6ca-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8d6ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d6ca-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d6ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d6ca-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d6ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d6ca-107">Remoteunterstützung anfordern</span><span class="sxs-lookup"><span data-stu-id="8d6ca-107">Request remote assistance</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d6ca-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d6ca-108">Prerequisites</span></span>
<span data-ttu-id="8d6ca-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d6ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d6ca-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d6ca-111">Permission type</span></span>|<span data-ttu-id="8d6ca-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d6ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d6ca-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d6ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d6ca-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d6ca-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8d6ca-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d6ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d6ca-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d6ca-116">Not supported.</span></span>|
|<span data-ttu-id="8d6ca-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d6ca-117">Application</span></span>|<span data-ttu-id="8d6ca-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d6ca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d6ca-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d6ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/requestRemoteAssistance
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="8d6ca-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d6ca-120">Request headers</span></span>
|<span data-ttu-id="8d6ca-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8d6ca-121">Header</span></span>|<span data-ttu-id="8d6ca-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8d6ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d6ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d6ca-123">Authorization</span></span>|<span data-ttu-id="8d6ca-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d6ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d6ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d6ca-125">Accept</span></span>|<span data-ttu-id="8d6ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d6ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d6ca-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d6ca-127">Request body</span></span>
<span data-ttu-id="8d6ca-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8d6ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d6ca-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d6ca-129">Response</span></span>
<span data-ttu-id="8d6ca-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="8d6ca-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8d6ca-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d6ca-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d6ca-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d6ca-132">Request</span></span>
<span data-ttu-id="8d6ca-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d6ca-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="8d6ca-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d6ca-134">Response</span></span>
<span data-ttu-id="8d6ca-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d6ca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





