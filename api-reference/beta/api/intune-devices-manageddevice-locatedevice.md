---
title: locateDevice-Aktion
description: Suchen eines Geräts
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2f7719fd2e306ceaa1169afebb54ee6cec5c6061
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868474"
---
# <a name="locatedevice-action"></a><span data-ttu-id="9b32d-103">locateDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="9b32d-103">locateDevice action</span></span>

> <span data-ttu-id="9b32d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9b32d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b32d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b32d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b32d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9b32d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b32d-107">Suchen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="9b32d-107">Locate a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b32d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9b32d-108">Prerequisites</span></span>
<span data-ttu-id="9b32d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b32d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b32d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9b32d-111">Permission type</span></span>|<span data-ttu-id="9b32d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9b32d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b32d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9b32d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b32d-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9b32d-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="9b32d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9b32d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b32d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b32d-116">Not supported.</span></span>|
|<span data-ttu-id="9b32d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9b32d-117">Application</span></span>|<span data-ttu-id="9b32d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b32d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b32d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b32d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/locateDevice
```

## <a name="request-headers"></a><span data-ttu-id="9b32d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b32d-120">Request headers</span></span>
|<span data-ttu-id="9b32d-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9b32d-121">Header</span></span>|<span data-ttu-id="9b32d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9b32d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b32d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b32d-123">Authorization</span></span>|<span data-ttu-id="9b32d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9b32d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b32d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9b32d-125">Accept</span></span>|<span data-ttu-id="9b32d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b32d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b32d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b32d-127">Request body</span></span>
<span data-ttu-id="9b32d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9b32d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b32d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b32d-129">Response</span></span>
<span data-ttu-id="9b32d-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="9b32d-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9b32d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b32d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b32d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b32d-132">Request</span></span>
<span data-ttu-id="9b32d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9b32d-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/locateDevice
```

### <a name="response"></a><span data-ttu-id="9b32d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b32d-134">Response</span></span>
<span data-ttu-id="9b32d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b32d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





