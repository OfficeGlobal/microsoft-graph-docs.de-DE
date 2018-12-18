---
title: requestRemoteAssistance-Aktion
description: Remoteunterstützung anfordern
author: tfitzmac
ms.openlocfilehash: d2668ff42571f285f7b7f40f0a514e42d78f9fd0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336806"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="28d5f-103">requestRemoteAssistance-Aktion</span><span class="sxs-lookup"><span data-stu-id="28d5f-103">requestRemoteAssistance action</span></span>

> <span data-ttu-id="28d5f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="28d5f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28d5f-105">Remoteunterstützung anfordern</span><span class="sxs-lookup"><span data-stu-id="28d5f-105">Request remote assistance</span></span>
## <a name="prerequisites"></a><span data-ttu-id="28d5f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="28d5f-106">Prerequisites</span></span>
<span data-ttu-id="28d5f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28d5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28d5f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28d5f-109">Permission type</span></span>|<span data-ttu-id="28d5f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28d5f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28d5f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28d5f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28d5f-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28d5f-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="28d5f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28d5f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28d5f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28d5f-114">Not supported.</span></span>|
|<span data-ttu-id="28d5f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28d5f-115">Application</span></span>|<span data-ttu-id="28d5f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28d5f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28d5f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28d5f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="28d5f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28d5f-118">Request headers</span></span>
|<span data-ttu-id="28d5f-119">Header</span><span class="sxs-lookup"><span data-stu-id="28d5f-119">Header</span></span>|<span data-ttu-id="28d5f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="28d5f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28d5f-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="28d5f-121">Authorization</span></span>|<span data-ttu-id="28d5f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="28d5f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28d5f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="28d5f-123">Accept</span></span>|<span data-ttu-id="28d5f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="28d5f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28d5f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28d5f-125">Request body</span></span>
<span data-ttu-id="28d5f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="28d5f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28d5f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="28d5f-127">Response</span></span>
<span data-ttu-id="28d5f-128">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="28d5f-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="28d5f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28d5f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="28d5f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28d5f-130">Request</span></span>
<span data-ttu-id="28d5f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28d5f-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="28d5f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="28d5f-132">Response</span></span>
<span data-ttu-id="28d5f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28d5f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



