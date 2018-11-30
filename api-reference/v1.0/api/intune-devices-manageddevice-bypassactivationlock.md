---
title: bypassActivationLock-Aktion
description: Aktivierungssperre umgehen
ms.openlocfilehash: 284efa6e1e15173ed028617334b5ee05237ad75f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018668"
---
# <a name="bypassactivationlock-action"></a><span data-ttu-id="1ce7d-103">bypassActivationLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="1ce7d-103">bypassActivationLock action</span></span>

> <span data-ttu-id="1ce7d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1ce7d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ce7d-105">Aktivierungssperre umgehen</span><span class="sxs-lookup"><span data-stu-id="1ce7d-105">Bypass activation lock</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ce7d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1ce7d-106">Prerequisites</span></span>
<span data-ttu-id="1ce7d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ce7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ce7d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ce7d-109">Permission type</span></span>|<span data-ttu-id="1ce7d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ce7d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ce7d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ce7d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ce7d-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1ce7d-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="1ce7d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ce7d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ce7d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ce7d-114">Not supported.</span></span>|
|<span data-ttu-id="1ce7d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ce7d-115">Application</span></span>|<span data-ttu-id="1ce7d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ce7d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ce7d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ce7d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/bypassActivationLock
```

## <a name="request-headers"></a><span data-ttu-id="1ce7d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ce7d-118">Request headers</span></span>
|<span data-ttu-id="1ce7d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1ce7d-119">Header</span></span>|<span data-ttu-id="1ce7d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1ce7d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ce7d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ce7d-121">Authorization</span></span>|<span data-ttu-id="1ce7d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1ce7d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ce7d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1ce7d-123">Accept</span></span>|<span data-ttu-id="1ce7d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1ce7d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ce7d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ce7d-125">Request body</span></span>
<span data-ttu-id="1ce7d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1ce7d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ce7d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ce7d-127">Response</span></span>
<span data-ttu-id="1ce7d-128">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="1ce7d-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1ce7d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ce7d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ce7d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ce7d-130">Request</span></span>
<span data-ttu-id="1ce7d-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ce7d-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/bypassActivationLock
```

### <a name="response"></a><span data-ttu-id="1ce7d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ce7d-132">Response</span></span>
<span data-ttu-id="1ce7d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ce7d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



