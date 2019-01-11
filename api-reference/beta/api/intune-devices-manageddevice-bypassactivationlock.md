---
title: bypassActivationLock-Aktion
description: Aktivierungssperre umgehen
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 27fc3bac809ca501a669c1a00e4fda3e4ed425ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870574"
---
# <a name="bypassactivationlock-action"></a><span data-ttu-id="4d07e-103">bypassActivationLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="4d07e-103">bypassActivationLock action</span></span>

> <span data-ttu-id="4d07e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4d07e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d07e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d07e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d07e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4d07e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d07e-107">Aktivierungssperre umgehen</span><span class="sxs-lookup"><span data-stu-id="4d07e-107">Bypass activation lock</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d07e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d07e-108">Prerequisites</span></span>
<span data-ttu-id="4d07e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d07e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d07e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d07e-111">Permission type</span></span>|<span data-ttu-id="4d07e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d07e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d07e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d07e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d07e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4d07e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="4d07e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d07e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d07e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d07e-116">Not supported.</span></span>|
|<span data-ttu-id="4d07e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d07e-117">Application</span></span>|<span data-ttu-id="4d07e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d07e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d07e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d07e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/bypassActivationLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/bypassActivationLock
```

## <a name="request-headers"></a><span data-ttu-id="4d07e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d07e-120">Request headers</span></span>
|<span data-ttu-id="4d07e-121">Header</span><span class="sxs-lookup"><span data-stu-id="4d07e-121">Header</span></span>|<span data-ttu-id="4d07e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4d07e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d07e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d07e-123">Authorization</span></span>|<span data-ttu-id="4d07e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d07e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d07e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4d07e-125">Accept</span></span>|<span data-ttu-id="4d07e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d07e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d07e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d07e-127">Request body</span></span>
<span data-ttu-id="4d07e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4d07e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d07e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d07e-129">Response</span></span>
<span data-ttu-id="4d07e-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="4d07e-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4d07e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d07e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d07e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d07e-132">Request</span></span>
<span data-ttu-id="4d07e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d07e-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/bypassActivationLock
```

### <a name="response"></a><span data-ttu-id="4d07e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d07e-134">Response</span></span>
<span data-ttu-id="4d07e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d07e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





