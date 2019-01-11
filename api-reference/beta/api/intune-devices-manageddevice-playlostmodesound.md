---
title: PlayLostModeSound Aktion
description: Remotesperre
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17d099a02ce42db71d1f64f4175ffd6166be97b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858065"
---
# <a name="playlostmodesound-action"></a><span data-ttu-id="8ad1e-103">PlayLostModeSound Aktion</span><span class="sxs-lookup"><span data-stu-id="8ad1e-103">playLostModeSound action</span></span>

> <span data-ttu-id="8ad1e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ad1e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ad1e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ad1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ad1e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8ad1e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ad1e-107">Remotesperre</span><span class="sxs-lookup"><span data-stu-id="8ad1e-107">Remote lock</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ad1e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8ad1e-108">Prerequisites</span></span>
<span data-ttu-id="8ad1e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ad1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ad1e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ad1e-111">Permission type</span></span>|<span data-ttu-id="8ad1e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ad1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ad1e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ad1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ad1e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="8ad1e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="8ad1e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ad1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ad1e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ad1e-116">Not supported.</span></span>|
|<span data-ttu-id="8ad1e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ad1e-117">Application</span></span>|<span data-ttu-id="8ad1e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ad1e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ad1e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ad1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/playLostModeSound
```

## <a name="request-headers"></a><span data-ttu-id="8ad1e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ad1e-120">Request headers</span></span>
|<span data-ttu-id="8ad1e-121">Header</span><span class="sxs-lookup"><span data-stu-id="8ad1e-121">Header</span></span>|<span data-ttu-id="8ad1e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8ad1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ad1e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ad1e-123">Authorization</span></span>|<span data-ttu-id="8ad1e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8ad1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ad1e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8ad1e-125">Accept</span></span>|<span data-ttu-id="8ad1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ad1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ad1e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ad1e-127">Request body</span></span>
<span data-ttu-id="8ad1e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8ad1e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ad1e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ad1e-129">Response</span></span>
<span data-ttu-id="8ad1e-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="8ad1e-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8ad1e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ad1e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ad1e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ad1e-132">Request</span></span>
<span data-ttu-id="8ad1e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ad1e-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/playLostModeSound
```

### <a name="response"></a><span data-ttu-id="8ad1e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ad1e-134">Response</span></span>
<span data-ttu-id="8ad1e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ad1e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





